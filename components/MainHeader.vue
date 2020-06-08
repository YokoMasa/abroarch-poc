<template>
    <div class="headerWrapper">
        <div class="header">
            <div class="header-logo">
                <span class="header-logo-text">Abroarch</span>
            </div>
            <div class="header-menuWrapper">
                <a href="https://studio.creww.me/projects/22/" class="header-menu">Project Info</a>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped lang="scss">
$header-textColor: #555;

.headerWrapper {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 80px;
    background: white;
    z-index: 1;
}

.header {
    max-width: 1100px;
    height: 100%;
    margin-left: auto;
    margin-right: auto;
    position: relative;
    display: flex;
    flex-direction: space-between;

    &-logo {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 200px;
        height: 100%;

        &-text {
            font-size: 22pt;
            font-weight: 700;
            color: $header-textColor;
        }
    }

    &-menuWrapper {
        position: absolute;
        right: 0;
        width: 600px;
        height: 100%;
        margin-top: auto;
        margin-bottom: auto;
        display: flex;
        flex-direction: row-reverse;
        align-items: center;
    }

    &-menu {
        text-decoration: none;
        font-size: 14pt;
        color: $header-textColor;
        margin: 0 25px;
    }

    &-menu:hover {
        color: #9999cc;
        cursor: pointer;
    }
}
</style>