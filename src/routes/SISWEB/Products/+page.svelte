<script>
    import Table from "../Products/Table.svelte";

    let headers = [
        "ID",
        "TYPE",
        "NAME",
        "PRICE",
        "IN STOCK",
        "IMAGE",
        " ",
        " ",
    ];
    let data = [
        {
            id: "COS01",
            type: "Cosmetic",
            name: "Sephora Skin Care - 1 u",
            price: "$45.5",
            in_stock: 4,
        },
        {
            id: "CLE02",
            type: "Cleaning",
            name: "Windex - 45 oz",
            price: "$23.0",
            in_stock: 23,
        },
        {
            id: "BEA03",
            type: "Beauty",
            name: "Sephora Skin Care - 1 u",
            price: "$12.6",
            in_stock: 12,
        },
    ];

    

</script>

<main id="main">
    <h1>Products</h1>

    <hr />

    
        <button onclick="window.location.href='/SISWEB/Products/New';" class="add"><p>ADD PRODUCT</p></button>
        
    <hr />

    <Table {headers} {data} />

</main>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Gothic+A1:wght@100&family=Inter&family=Source+Sans+Pro&display=swap");

    #main {
        margin: auto;
        width: 90%;
    }

    

    .add {
        margin: 10px 10px;
        background: transparent;
        border-radius: 4px;
        border: 1px solid #7749F8;
        width: 253.22px;
        height: 38px;
        color: #7749F8;
        font-size: 18px;
        font-weight: 600px;
        cursor: pointer;
    }

    .add p {
        padding-top: 4px;
        }
    
</style>
