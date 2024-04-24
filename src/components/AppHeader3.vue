<template>
    <nav class="navbar navbar-expand-sm bg-info navbar-dark">
        <a href="/" class="navbar-brand">Quản lý mượn sách</a>
        <div class="mr-auto navbar-nav">
            <div class="nav-item">
                <router-link :to="{ name: 'bookmanager' }" class="nav-link">
                    Sách <i class="fas fa-book"></i>
                </router-link>
            </div>
            <div class="nav-item">
                <router-link :to="{ name: 'nxbmanager' }" class="nav-link">
                    Nhà xuất bản <i class="fas fa-building"></i>
                </router-link>
            </div>
        </div>
    </nav>
</template>