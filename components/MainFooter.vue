<template>
    <span>
        <div class="footer">
                <div class="col-12 col-sm-4"><div>&copy Sunray Church of Christ 2022</div></div>
                <div class="col-12 col-sm-4"><a href="http://maps.apple.com/?daddr=700+S+Ave+N,+Sunray+TX">7th & Ave N, Sunray, Texas 79086</a></div>
                <div class="col-12 col-sm-4"><a href="tel:806-948-4443">806-948-4443</a></div>
        </div>
    </span>

            <!-- <a href="http://maps.apple.com/?daddr=700+S+Ave+N,+Sunray+TX">7th & Ave N, Sunray, Texas 79086</a>
            <span class="dot">|</span>
            <a href="tel:806-948-4443">806-948-4443</a>
            <span class="dot">|</span>
            <span>&copy Sunray Church of Christ 2022</span> -->
</template>
	
<script setup>

</script>
	
<style lang="scss" scoped>

@import '../Assets/variables.scss';
.footer{
    width: 100%;
    min-height: 80px;
    background: $primary-bg;
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-wrap: wrap;
    text-align: center;
    @media only screen and (max-width: 660px) {
        font-size: .75rem;
    }
}

.footer>a{
    color: $primary;
}
.footer>a:hover{
    color: adjust-color($color: $primary, $lightness: 20%);
}
.dot{
    font-size: 2rem;
}
	
</style>