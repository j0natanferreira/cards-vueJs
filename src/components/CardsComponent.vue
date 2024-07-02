<template>
  <div class="cards">
    <div class="card-img">
      <div class="img">
        <img :src="avatar" alt="avatar" />
      </div>
    </div>
    <div class="card-info">
      <h3>{{ name }}</h3>
      <p>
        {{ description }}
      </p>
      <button>View More</button>
    </div>
  </div>
</template>
<script>
export default {
  name: "CardsComponent",
  props: {
    avatar: String,
    name: String,
    description: String,
  },
};
</script>

<style scoped>
.cards {
  width: 250px;
  height: 300px;
  border-radius: 20px;
  margin: 10px;
  background: #3d6ee5;
  transition: 0.3s ease-in-out;
}

.cards:hover {
  transform: translateY(-10px);
  box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.1);
}

.card-img {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 50%;
}

.card-img > .img {
  display: flex;
  align-items: center;
  justify-content: center;
  border: 2px solid #ffffff;
  border-radius: 100%;
  padding: 2px;
}

.card-img > .img > img {
  width: 90px;
  height: 90px;
  border-radius: 100%;
}

.card-info {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  text-align: center;
  gap: 4px;
  padding: 10px;
  width: 100%;
  height: 50%;
  background-color: #ffffff;
  border-radius: 20px;
}

.card-info > p {
  font-size: 16px;
  color: grey;
}

.card-info > button {
  background-color: #3d6ee5;
  color: #ffffff;
  border: none;
  border-radius: 4px;
  padding: 8px 14px;
  cursor: pointer;
  transition: 0.3s ease-in-out;
}

.card-info > button:hover {
  background-color: #5680ea;
}
</style>