<script setup>
import Books from './components/Books.vue'

  let books = [
  {
    id: 1,
    title: "History of Europe",
    cover:
      "https://printpress.cmsmasters.net/default/wp-content/uploads/sites/11/2019/05/printpress-product-6-540x861.jpg",
    isRead: true,
    isbn: "0-395-07157-8",
    author: "Daniel Trejo",
  },
  {
    id: 2,
    title: "Penguin Classics",
    cover:
      "https://printpress.cmsmasters.net/default/wp-content/uploads/sites/11/2019/05/printpress-product-2-540x861.jpg",
    isRead: false,
    isbn: "0-395-07157-8",
    author: "Daniel Trejo, Jon Snow",
  },
  {
    id: 3,
    title: "Becoming",
    cover:
      "https://printpress.cmsmasters.net/default/wp-content/uploads/sites/11/2019/05/printpress-product-7-540x861.jpg",
    isRead: false,
    isbn: "0-395-07157-8",
    author: "Daniel Trejo",
  },
  {
    id: 4,
    title: "Sonnets",
    cover:
      "https://printpress.cmsmasters.net/default/wp-content/uploads/sites/11/2019/05/printpress-product-5-540x861.jpg",
    isRead: false,
    isbn: "0-395-07157-8",
    author: "Daniel Trejo",
  },
]
  
</script>

<template>

  <div class="container">
    <h1>📖 Meus Livros</h1>
    <div class="header-btns">
      <button
        class="btn"
        
      >
        Adicionar Livro +
      </button>
    </div>
 
    <div class="books-container">
      <Books :books="books" />
      
    </div>
  </div>
</template>



<!-- <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css"
    integrity="sha512-KfkfwYDsLkIlwQp6LFnl8zNdLGxu9YAA1QvwINks4PhcElQSvqcyVLLD9aMhXd13uQjoXtEKNosOWaZqXgel0g=="
    crossorigin="anonymous" referrerpolicy="no-referrer" />
    <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/js/all.min.js"
      integrity="sha512-6PM0qYu5KExuNcKt5bURAoT6KCThUmHRewN3zUFNaoI6Di7XJPTMoT6K0nsagZKk2OB4L7E3q1uQKHNHd4stIQ=="
      crossorigin="anonymous" referrerpolicy="no-referrer"></script> -->