<template>
  <div>
    <p>Componente de mensagem</p>
    <div>
        <form id="shoes-form">
            <div class="input-container">
                <label for="nome">Nome do Cliente:</label>
                <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite seu nome!">
            </div>

            <div class="input-container">
                <label for="pao">Escolha seu tenis</label>
                <select name="pao" id="pao" v-model="pao">
                    <option value="">Escolha o tenis</option>
                    <option value="Integral">De cria</option>
                </select>
            </div>

            <div id="opcionais-container" class="input-container">
                <label id="opcionais-title" for="opcionais">Selecione os opcionais</label>
                <div class="checkbox-container">
                    <input type="checkbox" name="opcionais" v-model="opcionais" value="Street">
                    <span>Street</span>
                </div>
            </div>
            <div class="input-container">
                <input type="submit" class="submit-btn" value="Criar meu tenis">
            </div>

        </form>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
/* Vai para o centro da tela no maximo que der */
#shoes-form{
    max-width: 400px;
    margin: 0 auto;
}

/* Coloca o label numa linha e o campo abaixo da linha */
.input-container{
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
}

label { 
    font-weight: bold;
    margin-bottom: 15px;
    color: #222;
    padding: 5px 10px;
    border-left: 4px solid #FCBA03;
}

input, select {
    padding: 5px 10px;
    width: 300px;
}

#opcionais-container{
    flex-direction: row;
    flex-wrap: wrap;
}

#opcionais-title{
    width: 100%;
}

.checkbox-container{
    display: flex;
    align-items: flex-start;
    width: 50%;
    margin-bottom: 20px;
}

.checkbox-container span,
.checkbox-container input{
    width: auto;
}

.checkbox-container span{
    margin-left: 6px;
    font-weight: bold;
}
.submit-btn{
    background-color: #222;
    color: #FCBA03;
    font-weight: bold;
    border: 2px solid #222;
    padding: 10px;
    font-size: 16px;
    margin: 0 auto;
    cursor: pointer;
    transition: .5s;
}

.submit-btn:hover {
    background-color: transparent;
    color: #222;
}
</style>