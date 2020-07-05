<template>
    <div class="row">
        <div class="col">
            <div class="mt-5">
                <p class="size">Plazo Estimado:</p>
                <P>Indica el tiempo aproximado en el que necesitarás que se repita tu proyecto. Luego podrás precisarlo o revisarlo con mayor exactitud.</P>
            </div> 
            <!-- cards -->
                <div class="text-center card-group card-deck">
                    <div class="card">
                        <button
                            class="btn carta shadow tam"
                            @click="activar"
                        >
                            <div class="card-title">
                                <h5>1 a 7 Días</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar">
                            <div class="card-title">
                            <h5>8 a30 días</h5>
                            </div>
                        </button>
                    </div>
                    <div class="card">
                        <button class="btn btn carta shadow tam" @click="activar">
                            <div class="card-title">
                            <h5>Más de 30 días</h5>
                            </div>
                        </button>
                    </div>

                </div>

            
        </div>
    </div>
</template>

<style scoped>
.tam {
    height: 50px;
}
.carta:focus{
    background: #00a2c2;;
    color: white;
}
p {
    font-size: 18px;
}
.size {
    font-size: 24px;
}
</style>