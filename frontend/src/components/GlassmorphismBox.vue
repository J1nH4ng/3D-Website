<template>
    <div class="glass-morphism-container">
        <div class="icon-placeholder">
            <img :src="iconPath" alt="icon"/>
        </div>
    </div>
</template>

<script>
    export default {
        name: "GlassMorphismBox",
        props: {
            iconPath:  {
                type: String,
                required: true
            }
        }
    }
</script>

<style scoped>
.glass-morphism-container {
    width:150px;
    height: 150px;
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
    border-radius: 15px;
    border: 2px  solid rgba(255, 255, 255, 0.2);
    box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
    display: flex;
    justify-content: center;
    align-items: center;
}

.icon-placeholder {
    width: 80px;
    height: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.icon-placeholder img {
    width: 100%;
    height: 100%;
    object-fit: contain;
}
</style>