<script>
  let standings = [
    { name: 'Team A', points: 10 },
    { name: 'Team B', points: 8 }
  ];
</script>

<h2>Team Standings</h2>
<ul>
  {#each standings as team}
    <li>{team.name} - {team.points} points</li>
  {/each}
</ul>