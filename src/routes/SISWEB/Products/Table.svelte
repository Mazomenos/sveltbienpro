<script>
  let mostrarModal = false;

  function abrirModal() {
    mostrarModal = true;
  }

  function cerrarModal() {
    mostrarModal = false;
  }

  export let headers = [];
  export let data = [];
</script>

<div>
  {#if mostrarModal}
    <div class="fondo" on:click={cerrarModal} />
    <div class="ventana-modal">
      <h2>Delete Product</h2>
      <hr />
      <p>Are you sure you want to delete this product?</p>
      <div class="row">
        <div class="col">
          <button id="cancel" on:click={cerrarModal}>CANCEL</button>
        </div>
        <div class="col">
          <button id="delete" on:click={cerrarModal}>DELETE</button>
        </div>
      </div>
    </div>
  {/if}
</div>

<table class="table">
  <thead>
    <tr>
      {#each headers as header}
        <th>{header}</th>
      {/each}
    </tr>
  </thead>
  <tbody>
    {#each data as row}
      <tr>
        {#each Object.values(row) as value}
          <td>{value}</td>
        {/each}
        <td id="button"
          ><button><i id="image" class="fa-regular fa-image" /></button></td
        >
        <td
          ><a href="Products/Edit"
            ><button><i class="fa-solid fa-pen" /></button></a
          ></td
        >
        <td
          ><button on:click={abrirModal}
            ><i class="fa-regular fa-trash-can" /></button
          >
        </td>
      </tr>
    {/each}
  </tbody>
</table>

<style>
  hr{
    width: 100%;
  }

  h2 {
    font-family: "Inter";
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    line-height: 19px;

    color: #000000;
  }

  div p {
    font-family: "Inter";
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 26px;
    color: #6c757d;
  }

  table td {
    padding-top: 1%;
    padding-right: 1%;
    padding-bottom: 1%;
    padding-left: 1%;
  }

  table thead th {
    padding-top: 1%;
    padding-right: 10%;
    padding-bottom: 1%;
    padding-left: 1%;

    left: 73.54%;
    right: 22.71%;
    top: 32.32%;
    bottom: 65.54%;

    font-family: "Inter";
    font-style: normal;
    font-weight: 800;
    font-size: 16px;
    line-height: 19px;

    /* Heading/Title Color */

    color: #152536;
    border-bottom: 2px solid #dee2e6;
  }
  table tr {
    border-bottom: 1px solid #dee2e6;
  }
  table button {
    background-color: white;
    border: 0px solid white;
    padding: 0%;
  }
  table i {
    color: blueviolet;
    background-color: white;
  }
  #image {
    color: black;
  }

  .fondo {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    z-index: 1;
  }

  .ventana-modal {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 50%;
    height: 177px;
    padding: 0px;
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #fff;
    padding: 20px;
    z-index: 2;
    border-radius: 12px 12px 12px 12px;
  }

  div.row {
    display: flex;
    margin: auto;
    margin-left: 60%;
  }

  #cancel {
    background: #6c757d;
    border-radius: 4px;
    color: white;
    width: 100%;
    height: 39px;
    font-family: "Inter";
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    line-height: 19px;
    text-align: center;
  }
  #delete {
    background: #7749f8;
    border-radius: 4px;
    color: white;
    width: 100%;
    height: 39px;
    font-family: "Inter";
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    line-height: 19px;
    text-align: center;
  }
</style>
