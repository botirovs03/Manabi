<template>
  <div class="container">
    <div id="persona">
      <div>
        <img src="/public/images/Pers.png" />
      </div>
    </div>
    <div id="levels">
      <div class="active">N5</div>
      <div>N4</div>
      <div>N3</div>
      <div>N2</div>
      <div>N1</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
.container {
  margin-top: 24px;
  display: flex;
  width: 100%;
}

#persona {
  flex: 60%;
  display: flex;
  justify-content: center;
  align-items: center;
}

#persona img {
  height: 60vh;
}

#levels {
  flex: 40%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

#levels div {
    width: 60%;
    text-align: center;
    background-color: #CCCCCC;
    margin: 10px;
    padding: 10px;
    border-radius: 12px;
    font-size: 24px;
    user-select: none;
}

#levels div:hover {
 transform: scale(1.05);
}

#levels div:active {
 transform: scale(0.95);
}
#levels div.active {
    background-color: #FFFFFF;
}
</style>