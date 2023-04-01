

<main id="main">
    <h1>Edit Product</h1>

    <hr />

    <form>
        <div class="container">
            <div class="row">
                <div class="col-sm-3">
                    <label for="myfile">Image</label><br />
                    <img
                        src="https://www.macmillandictionary.com/external/slideshow/thumb/Grey_thumb.png"
                        alt=""
                    />
                    <div class="input-group mb-3">
                        <input
                            type="text"
                            class="form-control"
                            placeholder="Select file from local drive"
                        />
                        <button class="btn" type="button">Browse</button>
                    </div>
                </div>
                <div class="col">
                    <div class="row">
                        <div class="col">
                            <label for="id">ID</label><br />
                            <div class="input-group input-group mb-3">
                                <input
                                    type="text"
                                    class="form-control"
                                    id="id"
                                    name="id"
                                    disabled
                                />
                            </div>
                        </div>
                        <div class="col">
                            <label for="type">Type</label><br />
                            <select name="type" id="type">
                                <option value="1" />
                                <option value="2">Cosmetic</option>
                                <option value="3">Cleaning</option>
                                <option value="4">Beauty</option>
                            </select><br />
                        </div>
                    </div>
                    <label for="name">Name:</label><br />
                    <div class="input-group input-group mb-3">
                        <input
                            type="text"
                            class="form-control"
                            id="name"
                            name="name"
                        />
                    </div>
                    <div class="row">
                        <div class="col">
                            <label for="price">Price</label><br />
                            <div class="input-group input-group mb-3">
                                <input
                                    type="number"
                                    class="form-control"
                                    id="price"
                                    name="price"
                                />
                                <span class="input-group-text">USD</span>
                            </div>
                        </div>
                        <div class="col">
                            <label for="id">In Stock</label><br />
                            <div class="input-group input-group mb-3">
                                <input
                                    type="number"
                                    class="form-control"
                                    id="in_stock"
                                    name="in_stock"
                                />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <br />
        <hr />
        <br />
        <br />
        <a href="/SISWEB/Products"><input id="cancel" type="reset" value="CANCEL" /></a>
        <input id="update" type="submit" value="UPDATE" />
    </form>
</main>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Gothic+A1:wght@100&family=Inter&family=Source+Sans+Pro&display=swap");
    div.container {
        width: 100%;
    }
    h1 {
        font-family: "Inter";
        font-style: normal;
        font-weight: 700;
        font-size: 40px;
        line-height: 48px;
        letter-spacing: -0.02em;
    }
    #main {
        margin: auto;
        width: 90%;
    }

    img {
        width: 100%;
        height: 230px;
        display: flex;
        margin: auto;
        margin-top: 7px;
        margin-bottom: 33px;
    }

    form label {
        font-family: "Inter";
        font-style: normal;
        font-weight: 500;
        font-size: 18px;
        line-height: 22px;
    }

    form input {
        width: 20%;
        border: 1px solid #ced4da;
    }
    form select {
        width: 100%;
        height: 38px;
        border: 1px solid #ced4da;
        border-radius: 4px;
    }

    form div button {
        background-color: rgba(248, 249, 250, 1);
        border: 1px solid #ced4da;
    }
    #cancel {
        background: #6c757d;
        border-radius: 4px;
        color: white;
        width: 8%;
        height: 39px;
        font-family: "Inter";
        font-style: normal;
        font-weight: 600;
        font-size: 16px;
        line-height: 19px;
        text-align: center;
    }
    #update {
        background: #7749f8;
        border-radius: 4px;
        color: white;
        width: 8%;
        height: 39px;
        font-family: "Inter";
        font-style: normal;
        font-weight: 600;
        font-size: 16px;
        line-height: 19px;
        text-align: center;
    }
</style>
