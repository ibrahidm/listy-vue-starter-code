<template>
    <div class="sidebar">
        <div class="sidebar-title">
            Listy
        </div>
        <div class="sidebar-divider" />
        <div class="sidebar-content-slot">
            <!-- SidebarItem(s) go(es) here  -->
        </div>
        <div class="sidebar-action-slot">
            <input class="sidebar-add-field" 
                type="text" 
            />
            <input class="sidebar-add-button" 
                type="submit" 
            />
        </div>
    </div>
</template>

<script lang="ts">
export default {
    
}
</script>

<style scoped>
.sidebar {
    display: flex;
    flex-direction: column;
    justify-content: baseline;
    position: fixed;
    width: 270px;
    height: 100%;
    border-right: 1px solid #dfe1e5;
    background-color: #e8f0f2;
}

.sidebar-content-slot {
    flex: 1 1 auto;
    display: flex;
    flex-direction: column;
    overflow: auto;
    overflow-x: hidden;
    min-height: 120px;
}

.sidebar-title {
    font-size: 28px;
    align-self: center;
    margin: 15px;
    font-weight: 600;
}

.sidebar-divider {
    border-top: 1px solid #dfe1e5;
    padding-bottom: 8px;
}

.sidebar-action-slot {
    width: 100%;
    margin-bottom: 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.sidebar-add-field {
    margin-bottom: 8px;
    padding: 0 5px;
    width: 91%;
    border-top: 1px solid #dfe1e5;
    border-bottom: 1px solid #dfe1e5;
    border-left: none;
    border-right: none;
    border-radius: 2px;
    font-size: 20px;
    line-height: 1.7;
}

.sidebar-add-field:focus {
    box-shadow: 0 1px 6px rgb(32 33 36 / 28%);
    border-color: rgba(223, 225, 229, 0);
}

.sidebar-add-button {
    box-sizing: border-box;
    width: 100%;
    background-color: #a2dbfa;
    font-size: 20px;
    color: #053742;
    border: none;
    padding: 10px 0;
    cursor: pointer;
}

.sidebar-add-button:hover {
    background-color: #39a2db;
    color: white;
}
</style>
