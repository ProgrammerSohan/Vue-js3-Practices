<template lang="html">
    <div>
        <p class="header">Header</p>

            <slot>No Component Added.</slot>
        <p class="footer">Footer</p>
        <slot name="afterFooter"></slot>
        
    </div>
</template>
<script lang="js">
export default {
     name: "LayoutComponent"   

}
</script>
<style lang="css">
.header,
.footer{
    background-color: black;
    color:white;
    padding: 20px;

}

    
</style>