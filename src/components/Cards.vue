<template>
    <div class="homes">
      <div id="display">
  
      </div>
    </div>
  </template>
  
  <script>
  
    
    async function getData(){
      const data = await fetch('https://lc1007.github.io/jsonServer-Exercise/users.json')
      const formatData = await data.json()
  
      extractedData = formatData.students
  
      const display = document.querySelector('#display')
  
      extractedData.forEach(users =>{
      display.innerHTML += `
      <div class="card">
          <img src="https://images.pexels.com/photos/15286/pexels-photo.jpg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" style="width: 18rem" alt="">
          <div class="card-body">
            <h3 class="card-title">${users.first_name}</h3>
            <p class="card-text">${users.email}</p>
          </div>
        </div>
    `
  })
  }
  
  
    getData()
  
    
  
  </script>
  
  <style scoped>
    .homes{
      height: 310vh;
    }
  </style>

