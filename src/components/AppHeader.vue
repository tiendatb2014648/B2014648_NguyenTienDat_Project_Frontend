<template>
    <nav class="navbar navbar-expand-sm bg-info navbar-dark">
        <a href="/" class="navbar-brand">Quản lý mượn sách</a>
        <div class="navbar-nav">
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
            <div><button class="btn btn-danger" @click="logout"> Đăng xuất
                    <i class="fas fa-sign-out-alt"></i>
                </button></div>

        </div>
    </nav>
</template>

<script>
export default {
    methods: {
        logout() {
            // Thực hiện các thao tác để đăng xuất, ví dụ: xóa dữ liệu đăng nhập khỏi localStorage
            localStorage.removeItem('loggedInUser');
            // Sau đó chuyển hướng người dùng về trang đăng nhập hoặc trang chính
            this.$router.push({ name: 'manager' });
        }
    }
};
</script>