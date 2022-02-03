<template>
     <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-header">
                <h5 class="modal-title">{{character.name}}</h5>
                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">


                    <img :src="character.thumbnail"
                         class="img-fluid rounded-start"
                         :alt="character.name">
                    <div>
                        <h5>Описание</h5>
                        <p>
                            {{character.description}}
                        </p>
                        <h5>Комиксы</h5>
                        <ul>
                            <li>Amazing Spider-Man: Renew Your Vows #1-5 (2015) - лимитка в кроссовере.</li>
                            <li>Civil War #1-5 (2015) - лимитка.</li>
                            <li>   Future Imperfect #1-5 (2015) - лимитка.</li>
                            <li>Secret Wars: Battleworld #1-5 (2015) - лимитка.</li>
                            <li>Spider-Verse #1-5 (2015) - лимитка.</li>
                            <li>Ultimate End #1-5 (2015) - лимитка.</li>
                            <li>Secret Wars: Secret Love #1 (2015) - уан-шот.</li>
                        </ul>
                    </div>
                </div>
                <div class="modal-footer">
                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Закрыть</button>
                </div>
            </div>
            </div>
        </div>
</template>

<script>
    export default {
        name: "AppModal",
        props: ['character'],
    }
</script>

<style scoped>

</style>
