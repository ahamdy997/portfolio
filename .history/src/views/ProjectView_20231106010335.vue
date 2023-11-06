<template>
  <div>
    <h2>Project Title: Product Management System</h2>
    <h2>Description:</h2>
    <p>
      The Product Management System is a web-based CRUD application that allows
      users to efficiently manage and track product information, making it a
      valuable tool for businesses to maintain an organized product catalog.
      This project serves as a showcase of my frontend development expertise,
      emphasizing user interface design and user experience.
    </p>
    <ol>
      <h3>Key Features:</h3>
      <li>
        Create (Add Product): Users can easily add new products to the system,
        providing details such as product name, description, price, and product
        category.
      </li>
      <li>
        Read (View Product Data): The system enables users to search, filter,
        and view product data, making it simple to access essential information
        like product details, pricing, and availability.
      </li>
      <li>
        Update (Edit Product Information): Authorized users can edit product
        details, ensuring that product information remains up-to-date with
        changes in pricing, description, or availability.
      </li>
      <li>
        Delete (Remove Product): Users with appropriate permissions can remove
        product entries, with safeguards in place to prevent accidental
        deletions.
      </li>
    </ol>
    <div class="view">
      <button type="button">Review Project</button>
      <button type="button">Next Project</button>
    </div>
  </div>
</template>
<style scoped>
img {
  width: 100%;
}
div {
  text-align: left;
}

h2 {
  margin-bottom: 1.7rem;
  font-size: 3rem;
}
p {
  font-size: 1.7rem;
  margin-bottom: 1rem;
}
h3 {
  margin-bottom: 1rem;
  font-size: 1.7rem;
}

li {
  list-style-position: inside;
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
}
.view {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
button {
  background-color: #261c33;
  margin-top: 1.5rem;
  padding: 7px 20px;
  color: white;
  box-shadow: 1px 1px 5px white;
  border-radius: 20px;
}
</style>
