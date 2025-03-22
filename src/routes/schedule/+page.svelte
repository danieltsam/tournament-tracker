<script context="module" lang="ts">
  export async function load() {
    console.log('Load function called');
    const schedule = [
      ["Match 1", "10:00 AM", "Court 1"],
      ["Match 2", "10:45 AM", "Court 2"],
      ["Match 3", "11:30 AM", "Court 1"]
    ];

    console.log('Returning schedule:', schedule);

    return {
      props: {
        schedule
      }
    };
  }
</script>

<script lang="ts">
  export let schedule: string[][];
  console.log('Received schedule:', schedule);
</script>

<style>
  table {
    width: 100%;
    border-collapse: collapse;
  }
  th, td {
    padding: 10px;
    border: 1px solid #ddd;
  }
</style>

<h2>Tournament Schedule</h2>

{#if schedule && schedule.length > 0}
  <table>
    <thead>
      <tr>
        <th>Match</th>
        <th>Time</th>
        <th>Location</th>
      </tr>
    </thead>
    <tbody>
      {#each schedule as match}
        <tr>
          <td>{match[0]}</td> <!-- Match Name -->
          <td>{match[1]}</td> <!-- Time -->
          <td>{match[2]}</td> <!-- Location -->
        </tr>
      {/each}
    </tbody>
  </table>
{:else}
  <p>No schedule data available.</p>
{/if}