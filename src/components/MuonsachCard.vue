<script>
export default {
    props: {
        muonsach: { type: Object, required: true },
    },
};
</script>
<template>
    <div>
        <div class="p-1">
            <strong>Mã độc giả:</strong>
            {{ muonsach.madocgia }}
        </div>
        <div class="p-1">
            <strong>Mã sách:</strong>
            {{ muonsach.masach }} 
        </div>
        <div class="p-1">
            <strong>Ngày mượn:</strong>
            {{ muonsach.ngaymuon }}
        </div>
        <div class="p-1">
            <strong>Ngày trả:</strong>
            {{ muonsach.ngaytra }}

        </div>
    </div>
</template>