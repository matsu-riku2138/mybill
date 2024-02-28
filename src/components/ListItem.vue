<template>
    <div class="mt-3">
        <div class="m-auto mt-3 px-2" style="max-width: 800px;">
            <div v-for="item in items">
                <div class="input-group mb-1">
                    <!-- <div class="input-group-text">
                        <input class="form-check-input mt-0" type="checkbox" value="" aria-label="Checkbox for following text input">
                    </div>                 -->
                    <input type="text" class="form-control" placeholder="商品名" aria-label="name">
                    <span class="input-group-text">値段</span>
                    <input type="text" class="form-control" aria-label="Amount (to the nearest dollar)">
                    <span class="input-group-text">円</span>
                    <button class="btn btn-danger" type="button" id="button-addon2">削除</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            items: [1, 2]
        }
	}
}
</script>