<script>
    let data = { message: '' };
  
    async function fetchData() {
      const res = await fetch('http://localhost:3001/api/data');
      data = await res.json();
    }
  
    fetchData();
  </script>
  
  <main>
    <h1>sddd</h1>
    <h1>{data.message}</h1>
  </main>