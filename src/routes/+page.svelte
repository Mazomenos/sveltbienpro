<script>


</script>
    <div class=authContainer>
        <div class=formContainer>
            <form>
                <h1 class="title">WELCOME TO SISWEB</h1>
                <p class="subtitle">Please, sign in</p>

                <label> <p>Username</p>
                    <input type="Username"/>
                </label>
                <label> <p>Password</p>
                    <input type="Password"/>
                </label>

                <button onclick="window.location.href='/SISWEB/Products';">
                    <p>SIGN IN</p>
                </button>

            </form>
        </div>    
    </div>

<style>
    .authContainer {
        background: #7749F8;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        flex: 1;
        min-height: 100vh;

    }

    .title {
        font-weight: 700;
        line-height: 48.41px;
        width: 792px;
    }

    label p {
        padding-left: 4px;
        text-align: left;
        font-weight: 500;
        font-size: 18px;
        line-height: 21.78px;
        
    }

    input {
        width: 315px;
        height: 38px;
        margin-top: 6px;
        margin-bottom: 10px;
        border-radius: 4px;
        border: 1px solid #CED4DA;
        padding: 5px;
    }

    .subtitle {
        color: #B4B0B0;
        margin-bottom: 69px;
        font-weight: 500;
        font-size: 20;
        line-height: 24.2px;
    }

    .formContainer {
        background: white;
        border-radius: 4px;
        border: none;
        text-align: center;
        max-width: 792px;
        min-height: 494px;
        
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;

    }

    form {
        color: black;
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 315px;
    }

    form button {
        width: 186px;
        height: 39px;
        margin-top: 38px;
        margin-bottom: 61px;
        border-radius: 4px;
        border: none;
        background: #7749F8;
        color: white;
        cursor: pointer;
    }

    form button:hover {
        transform:scale(1.1);
        background: #6936f7;
    }

</style>