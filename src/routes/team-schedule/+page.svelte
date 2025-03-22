<script>
  export let params;
  let teamSchedule = [
    { date: '2025-03-24', opponent: 'Team B' },
    { date: '2025-03-25', opponent: 'Team C' }
  ];
</script>

<h2>Schedule for {params.team}</h2>
<ul>
  {#each teamSchedule as game}
    <li>{game.date} - {game.opponent}</li>
  {/each}
</ul>