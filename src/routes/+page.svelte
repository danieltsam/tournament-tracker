<!-- filepath: src/routes/+page.svelte -->
<script>
    let message = "Welcome to the Volleyball Tournament!";
  </script>
  
  <style>
    h2 {
      color: #2b2b2b;
    }
  
    p {
      font-size: 1.2rem;
    }
  </style>
  
  <h2>{message}</h2>
  <p>Check out the latest tournament schedule, standings, and team-specific schedules!</p>
  <ul>
    <li><a href="/schedule">Tournament Schedule</a></li>
    <li><a href="/standings">Standings</a></li>
    <li><a href="/team-schedule">Team Schedules</a></li>
  </ul>