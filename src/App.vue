<script setup>
const currentYear = new Date().getFullYear();
</script>
<template>
    <div class="app-height">
        <nav class="navbar navbar-expand bg-body border-bottom border-opacity-25 position-sticky sticky-top">
            <div class="container content-width">
                <a class="navbar-brand" href="/">
                    Tyler Grow<span class="d-none d-sm-inline"> &nbsp;&nbsp;·&nbsp;&nbsp; Accessibility
                        <span class="d-none d-md-inline">Certificate</span>
                    </span>
                </a>
                <div class="py-2 ps-3 pe-0">
                    <div class="d-flex my-2 my-lg-0">
                        <a class="btn btn-primary" target="_blank" href="./tylergrow_accessibility_certificate.pdf" download>Download PDF</a>
                    </div>
                </div>
            </div>
        </nav>


        <div class="container content-width app-height pt-5">
            <div class="app-height row justify-content-center pt-5 align-items-center">
                <div class="col-12">
                    <div class="card">

                        <div class="card-body px-4 px-lg-5 py-4">
                            <div class="col-12 pb-2">
                                <h1 class="h4 m-0 card-title">Accessibility Certificate for Tyler Grow</h1>
                                <p class="mt-3 mb-0">This certificate from <a href="https://webaim.org" target="__blank">WebAIM</a> is verification of completed accessibility training by Tyler Grow.</p>
                            </div>
                        </div>
                        <img src="./assets/tylergrow_accessibility_certificate.png" class="card-img-bottom" alt="Tyler Grow WebAIM Verification of Accessibility Training Certificate">
                    </div>
                </div>

            </div>
        </div>
    </div>
    <footer>
        <div class="container p-4">
            <div class="row justify-content-center">
                <div class="col-12">
                    <p class="text-center mb-0 d-block w-100 px-3">© {{ currentYear }} Tyler Grow</p>
                </div>
            </div>
        </div>
    </footer>
</template>
<style lang="scss" scoped>
@use "sass:math";
$iw: 8.5;
$ih: 11;
$img-ratio: math.percentage(math.div($ih, $iw));

.card {
    overflow: hidden;
    border-radius: 0.5rem;
}

.img-col {
    height: auto;
    flex: 1 1 auto;

    .img-outer {
        width: 100%;
        height: 0;
        padding-bottom: $img-ratio;
        position: relative;
        overflow: hidden;
        background-color: yellow;

        .img {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }
    }

}

// .card-title {
//     font-weight: 700;
//     font-size: 1.75rem;

//     margin-bottom: 1.75rem;
// }

// .card-subtitle {
//     font-weight: 400;
//     font-size: 1.375rem;
//     line-height: 1.5;
//     margin-bottom: 0;
// }

.content-col {
    display: flex;
    width: 100%;
    max-width: 440px;
    padding: 40px;
    justify-content: flex-start;
    align-items: space-between;
    flex-direction: row;
    flex-wrap: wrap;
    align-self: stretch;
    ;

    & > * {
        width: 100%;
    }
}

.app {
    width: 100vh;
    min-width: 100vh;
    max-width: 100vh;
    min-height: 100vh;
}

.container {
    .content-width {
        max-width: 850px;
        margin: 0 auto;
    }
}

.content-width {
    width: 100%;
    max-width: 850px;
    margin: 0 auto;
}

.app-height {
    min-height: 100vh;

}
</style>