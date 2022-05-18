<template>
  <nav id="primary_header_navigation">
    <ul>
      <li>
        <a href="#">Home</a>
      </li>
      <li>
        <a href="#">Books</a>
      </li>
      <li>
        <a href="#">Contacts</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'MainHeader',
  props: {
    msg: String
  }
}
</script>

<style lang="scss" scoped>
#primary_header_navigation{
  width:100%;
  position:sticky;
  top:0;
  background-color: rgba(0, 0, 0, 0.3);
  
    
  ul{
    display: flex ;
    align-content: center;
    justify-content: center;
    flex-wrap: nowrap;
    align-items: center;
    list-style: none;
    li{
      padding:1rem;
      
      a{
        color: black;
        text-decoration: none;
        font-size: 1.5rem;
        font-weight: 600;
      }
    }
  }
  
}
</style>
