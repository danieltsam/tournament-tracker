<script lang="ts">
	import '../app.css';
  </script>
  
  <style>
	header {
	  padding: 1rem;
	  background-color: thistle;
	  color: white;
	}
  
	footer {
	  padding: 1rem;
	  background-color: thistle;
	  color: white;
	  text-align: center;
	}
  
	main {
	  padding: 2rem;
	}
  </style>
  
  <header>
	<h1>Volleyball Tournament Tracker</h1>
  </header>
  
  <main>
	<slot></slot>
  </main>
  
  <footer>
	<p>© Built by danieltsam </p>
  </footer>