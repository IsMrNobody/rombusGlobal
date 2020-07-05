<template>
    <div>
<!-- Rango -->
        <div class="d-flex justify-content-end mt-5">
            <!-- Signo "?" -->
            <div class="d-flex justify-content-end mx-2">
                <span 
                    class="badge badge-light bk border border-dark rounded-circle ">
                    ?
                </span>
            </div>
            <form>
            <!-- Precios -->
                <div class="form-group">
                    <label>Rango de precio sugerido</label>
                    <input 
                    type="number" 
                    class="form-control form-control-lg" 
                    id="Input" 
                    placeholder="$ 1000/2.000">
                </div>

                <div class="form-group mt-4">
                    <label>Tu presupuesto</label>
                    <input 
                    type="number" 
                    class="form-control form-control-lg" 
                    id="Input2" 
                    placeholder="$">
                </div>
            </form> 
        </div>
    </div>
</template>

<style scoped>
.bk {
    height: 25px;
    width: 25px;
    margin-top: 3.5em;
    padding-left: 10px;
    align-items: center;
    display: flex;
}
</style>