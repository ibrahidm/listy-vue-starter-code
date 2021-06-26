<template>
    <div class="sidebar-item">
        <div class="sidebar-link">
            <!-- category.name goes here  -->
        </div>
        <transition name="slide">
            <div class="delete-button">
                Delete
            </div>
        </transition>
    </div>
</template>

<script lang="ts">

export default {
   
}
</script>

<style scoped>
    .sidebar-item {
        font-size: 20px;
        display: flex;
        flex: 0 0 auto;
        justify-content: center;
        align-items: center;
        background: #053742;
        color: white;
        margin-bottom: 5px;
        cursor: pointer;
        text-decoration: none;
    }

    .sidebar-item:hover {
        background: #053742b0;
    }

    .sidebar-link {
        display: flex;
        color: inherit;
        text-decoration: inherit;
        flex: 1 1;
        position: relative;
        padding: 12px;

    }

    .sidebar-link:hover {
        width: 50%;
        transition: width 0.4s;
    }

    .delete-button {
        font-size: 14px;
        height: 100%;
        display: flex;
        align-items: center;
        padding: 0px 10px;
        background: red;
    }

    .delete-button:hover {
        background: rgb(250, 106, 106);
    }

    .slide-enter-active {
        transition: all 0.4s;
    }

    .slide-leave-active {
        transition: all 0.4s;
    }

    .slide-enter-from,
    .slide-leave-to,
    .shrink-enter-from,
    .shrink-leave-to {
    transform: translateX(60px);
    }
</style>