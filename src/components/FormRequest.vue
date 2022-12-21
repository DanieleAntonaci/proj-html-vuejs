<script>
export default {

}
</script>

<template>
    <div >
        <form action="requestToJoing">
            <input type="text" name="Name" id="input-name" placeholder="Name">
            <input type="text" name="Email" id="input-email" placeholder="Email">
            <input type="text" name="Telephone" id="input-phone" placeholder="Telephone">
            <button type="submit"> APPLY NOW</button>
        </form>
    </div>

</template>

<style lang="scss" scoped>
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

form {
    margin: 30px 0;


    input {
        margin: 0 5px;
        width: calc((100% / 4) - 30px);
        height: 30px;
        background-color: #444d63;
        border: 0;
        padding: 0 8px;
        color: $thirdColor;
    }

    button {
        padding: 8px 40px;
        border-radius: 0;
        margin: 0 5px;
        background-color: $primaryColor;
        color: $thirdColor;
        border: 0;
        font-size: 10px;
        vertical-align: middle;
    }
}
</style>