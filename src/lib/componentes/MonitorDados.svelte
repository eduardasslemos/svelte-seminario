<script lang="ts">
    import { nave } from "../nave.svelte";
</script>

<article>
    <h2>1. DADOS DA NAVE</h2>
    <ul>
        <li>Nome: {nave.shipName}</li>
        <li>Piloto: {nave.emailPiloto || 'Não Registrado'}</li>
        <li>Tripulantes: {nave.tripulantes}</li>
        <li>Dobra: {nave.warp ? 'true (Ativa)' : 'false (Inativa)'}</li>
        <li>Em Voo: {nave.decolou ? 'true (sim)' : 'false (não)'}</li>
        <li class="destaque">Em Voo: {nave.decolou}</li>
    </ul>
</article>

<style>
    .destaque{
        color: #00e5ff;
    }
</style>