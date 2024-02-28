<template>
    <div class="container" id="contact">
        <div class="row m-auto" style="max-width: 600px;">
            <h2 class="pt-5 pb-3">お問い合わせ</h2>
            <div class="mb-3">
                <label for="exampleFormControlInput1" class="form-label">メールアドレス</label>
                <input type="email" class="form-control m-auto" id="exampleFormControlInput1" style="max-width: 600px;">
            </div>
            <div class="mb-3">
                <label for="exampleFormControlInput1" class="form-label">お名前</label>
                <input type="text" class="form-control m-auto" id="exampleFormControlInput1" style="max-width: 600px;">
            </div>
            <div class="mb-3">
                <label for="exampleFormControlTextarea1" class="form-label">お問い合わせ内容</label>
                <textarea class="form-control m-auto" id="exampleFormControlTextarea1" rows="5"  style="max-width: 600px;"></textarea>
            </div>
            <div class="mb-3 mt-1">
                <div class="submit-button">
                    <div class="d-grid gap-2 d-md-block text-center mt-1 m-auto" style="max-width: 100px;">
                        <button type="submit" class="btn btn-secondary rounded-pill">送信する</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
