<template>
 <div class="contact">
  <form action="action_page.php">

    <label for="fname">Nombre</label>
    <input type="text" id="fname" name="firstname" placeholder="Your name..">

    <label for="lname">Apellido</label>
    <input type="text" id="lname" name="lastname" placeholder="Your last name..">

    <label for="country">Pais</label>
    <select id="country" name="country">
      <option value="Chile">Chile</option>
      <option value="España">España</option>
      <option value="Argentina">Argentina</option>
    </select>

    <label for="subject">Subject</label>
    <textarea id="subject" name="subject" placeholder="Escribeme." style="height:24px"></textarea>

    <b-button variant="outline-danger" input type="submit">Enviar</b-button>

  </form>
</div>
</template>

<script>
export default {
  name: "ContactView"
}
</script>
<style>

</style>