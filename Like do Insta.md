

<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <title>andrezin cu</title>
    <style>
        main {

            user-select: none;
            color: rgb(143, 102, 109);
            display: flex;
            cursor: pointer;
            font-size: 25vh;
        }
        div{
            width: 20vh;
            height: 2S0vh;
            flex: none;
            position: relative;
            border: 0 none;
             transform: rotate(2deg) scale(.5);
            transition: .3s;
            /* transition: 300ms; */
            top: 300px;
            left: 650px;
        }

        div:first-child {
            width: 40vh;
            height: 40vh;
            flex: none;
            position: relative;
            border: 0 none;
            background-color: red;
            transform: rotate(41deg) scale(.5);
            transition: .3s;
            /* transition: 300ms; */
        }

        div:first-child:hover {
            background-color: red;
        }

        div:first-child:before,
        div:first-child:after {
            content: " ";
            background-color: inherit;
            width: 100%;
            height: 100%;
            position: absolute;
            border-radius: 50%;
        }

        div:first-child:before {
            top: -50%;
            left: 0%;
        }

        div:first-child:after {
            top: 0%;
            left: -50%;
        }
        
    </style>
</head>

<body>
    <main>
        <div> </div>
        <div></div>
        </div> Instagram
        
        
       

    
        
    </main>
    <script>
        const domMain = document.querySelector("main")
        // const domDivNum = document.querySelector("main div:last-child")
        const domDivNum = domMain.querySelector("div:last-child")
        let counter = 0
        domMain.addEventListener("click", () => {
            counter++
            domDivNum.innerHTML = counter
        })
    </script>
</body>

</html>
