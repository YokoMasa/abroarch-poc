<template>
    <div class="footerWrapper">
       <div class="content">
           <small>
               Copyright &#169; 2020 Abroarch
            </small>
       </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped lang="scss">
$primary: #2195f2;
$primaryLight: #6ec5ff;
$primaryDark: #0068bf;

.footerWrapper {
    height: 40px;
    padding: 5px;
    background: $primaryDark;
    color: white;
}

.content {
    max-width: 1100px;
    height: 100%;
    margin-left: auto;
    margin-right: auto;
    display: flex;
    align-items: flex-end;
}
</style>