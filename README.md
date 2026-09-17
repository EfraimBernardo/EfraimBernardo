<!DOCTYPE html>
<html>
    <head>
        <title>Portfólio Profissional</title>
        <meta charset="UTF-8">
        <link rel="stylesheet" href="style.css">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css" integrity="sha512-2SwdPD6INVrV/lHTZbO2nodKhrnDdJK9/kg2XD1r9uGqPo1cUbujc+IYdlYdEErWNu69gVcYgdxlmVmzTWnetw==" crossorigin="anonymous" referrerpolicy="no-referrer" />

      <style>
          *{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,sans-serif;
    transition:.35s;
}

html{
    scroll-behavior:smooth;
}

body{
    background:rgb(23,30,40);
    color:#ddd;
    overflow-x:hidden;
}

body.claro{
    background:whitesmoke;
}

body.claro .card{
    background:whitesmoke;
}

body.claro .card img{
    border:1px solid #000;
}

body.claro .card h3,
body.claro .card p{
    color:rgb(23,30,40);
}

body.claro .card a{
    color:blue;
}

/* HEADER */

.mainHead{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:1000;

    display:flex;
    justify-content:space-between;
    align-items:center;

    padding:20px 70px;

    background:#171E28;
}

.messHead{
    width:100%;

    display:flex;
    justify-content:space-between;
    align-items:center;

    gap:30px;
    min-width:0;
}

.logo{
    font-size:clamp(18px,2vw,22px);
    font-weight:bold;

    color:#777;

    border-bottom:1px solid rgba(60,227,22,.9);

    white-space:nowrap;
}

.menu{
    display:flex;
    align-items:center;
    justify-content:flex-end;

    gap:30px;

    flex-wrap:wrap;

    min-width:0;
}

.menu a{
    color:#777;
    text-decoration:none;
    font-size:16px;

    white-space:nowrap;
}

.menu a:hover{
    color:#fff;
    border-bottom:1px solid rgba(60,227,22,.9);
}

.modo{
    cursor:pointer;
}

/* MAIN */

main{
    display:flex;
    justify-content:center;

    margin-top:120px;

    padding:20px;
}

.principal{
    background:rgb(25,35,49);

    width:100%;
    max-width:1700px;

    padding:40px;

    border-radius:14px;

    outline:.5px solid rgba(255,255,255,.2);

    min-width:0;
}

/* MESSAGE */

.message{
    position:fixed;

    top:0;
    left:0;

    width:100%;
    height:100%;

    background:rgba(0,0,0,.6);

    display:flex;
    justify-content:center;
    align-items:center;

    opacity:0;
    pointer-events:none;

    padding:20px;
}

.message.send{
    opacity:1;
    pointer-events:auto;
    z-index:9999;
}

.message div{
    background:rgb(23,30,40);

    width:100%;
    max-width:420px;

    padding:25px;

    border-radius:12px;

    display:flex;
    flex-direction:column;
    gap:15px;
}

.message input{
    width:100%;
    height:45px;

    border:none;
    outline:none;

    border-radius:6px;

    padding:10px;
}

.message button{
    width:100%;
    height:45px;

    border:none;

    border-radius:6px;

    cursor:pointer;
}

/* TEXTOS */

.intro{
    color:#777;
    margin-bottom:12px;
}

h1{
    font-size:clamp(2rem,5vw,3rem);
    margin-bottom:15px;

    overflow-wrap:break-word;
}

h2{
    font-size:clamp(1.5rem,3vw,2rem);

    overflow-wrap:break-word;
}

h3{
    color:#aaa;
    font-size:clamp(1rem,2vw,1.3rem);
    margin-bottom:20px;

    overflow-wrap:break-word;
}

p{
    line-height:1.7;

    overflow-wrap:break-word;
}

/* BOTAO */

.see{
    background:rgb(57,57,154);

    color:#fff;

    padding:13px 28px;

    border:none;

    border-radius:8px;

    cursor:pointer;

    margin-bottom:45px;

    max-width:100%;
}

.see:hover{
    transform:translateY(-2px);
}

/* SOBRE */

.sobre{
    margin-bottom:50px;

    min-width:0;
}

.sobre h2{
    margin-bottom:12px;
}

.sobre p{
    color:#aaa;
    line-height:1.8;
    font-size:clamp(.95rem,2vw,1.05rem);
}

/* PROJETOS */

.projetos{
    margin-top:20px;

    min-width:0;
}

.projetos h2{
    margin-bottom:20px;
}

.cards{
    display:grid;

    grid-template-columns:repeat(3,minmax(0,1fr));

    gap:25px;

    width:100%;
}

.card{
    background:#1e2a38;

    padding:20px;

    border-radius:12px;

    opacity:.8;

    outline:1px solid rgba(60,227,22,.9);

    overflow:hidden;

    min-width:0;
}

.card:hover{
    opacity:1;

    transform:translateY(-6px);

    box-shadow:0 10px 25px rgba(0,0,0,.35);
}

.card img{
    display:block;

    width:100%;

    aspect-ratio:16/9;

    object-fit:cover;

    border-radius:8px;

    margin-bottom:15px;
}

.card h3{
    margin-bottom:10px;
}

.card p{
    color:#aaa;

    margin-bottom:15px;

    line-height:1.7;
}

.card a{
    color:#4da6ff;

    text-decoration:none;

    font-weight:bold;

    overflow-wrap:anywhere;
}

.card a:hover{
    text-decoration:underline;
}

/* TECNOLOGIAS */

.tech-card{
    display:flex;

    flex-wrap:wrap;

    gap:10px;

    margin-top:15px;

    min-width:0;
}

.tech-card div{
    display:flex;

    justify-content:center;
    align-items:center;

    min-width:90px;

    padding:8px 12px;

    background:rgb(23,30,40);

    border-radius:8px;

    outline:1px solid rgba(60,227,22,.9);

    font-weight:bold;
}

.tech-card div:hover{
    background:rgba(60,227,22,.9);

    outline:1px solid #ddd;

    color:#111;

    cursor:default;

    transform:translateY(-2.5px);
}

/* CONTATO */

.contato{
    margin-top:60px;

    display:flex;

    flex-wrap:wrap;

    gap:15px;

    min-width:0;
}

.contato h2{
    margin-bottom:20px;
}

.contato button{
    flex:1 1 180px;

    color:#fff;

    padding:12px 20px;

    border:none;

    border-radius:8px;

    cursor:pointer;

    min-width:0;
}

button{
    background:rgb(23,30,40);

    outline:1px solid rgba(60,227,22,.9);
}

.botoes{
    display:flex;

    flex-wrap:wrap;

    gap:15px;

    margin-top:20px;

    width:100%;
}

.botoes button{
    flex:1 1 180px;

    color:#fff;

    padding:12px 20px;

    border:none;

    border-radius:8px;

    cursor:pointer;

    min-width:0;
}

.botoes button:hover{
    background:rgba(60,227,22,.9);

    outline:1px solid #ddd;

    color:#111;
}

.contato li{
    list-style:none;

    display:inline-flex;

    justify-content:center;
    align-items:center;

    padding:10px;

    font-size:clamp(26px,5vw,34px);

    cursor:pointer;
}

.nv{
    display:flex;

    justify-content:space-between;
    align-items:center;

    gap:20px;

    margin-bottom:20px;

    min-width:0;
}

.nv img{
    flex-shrink:0;

    width:60px;
    height:60px;

    border-radius:50%;

    object-fit:cover;

    outline:1px solid rgba(60,227,22,.9);
}

@media (max-width:1024px){

    .mainHead{
        padding:18px 30px;
    }

    .messHead{
        gap:20px;
    }

    .menu{
        gap:20px;
    }

    main{
        margin-top:120px;
        padding:20px;
    }

    .principal{
        width:100%;
        padding:30px;
    }

    .cards{
        grid-template-columns:repeat(2,minmax(0,1fr));
        gap:20px;
    }

    .card{
        min-width:0;
    }

    .contato{
        flex-wrap:wrap;
    }
}

@media (max-width:1024px){

    .mainHead{
        padding:20px 30px;
    }

    .messHead{
        gap:20px;
    }

    .menu{
        gap:20px;
    }

    .principal{
        width:100%;
    }

    .cards{
        grid-template-columns:repeat(2,1fr);
    }

}

@media (max-width:768px){

    .mainHead{
        padding:18px 20px;
    }

    .messHead{
        flex-wrap:wrap;
        gap:15px;
    }

    .menu{
        justify-content:flex-end;
        gap:15px;
    }

    .menu a{
        font-size:15px;
    }

    main{
        margin-top:120px;
        padding:15px;
    }

    .principal{
        padding:30px;
    }

    .cards{
        grid-template-columns:repeat(2,1fr);
        gap:20px;
    }

    .card{
        padding:18px;
    }

    h1{
        font-size:2.4rem;
    }

    h2{
        font-size:1.7rem;
    }

    h3{
        font-size:1.15rem;
    }

    .sobre p{
        font-size:1rem;
    }

    .contato{
        flex-wrap:wrap;
    }

    .botoes{
        flex-wrap:wrap;
    }

}

@media (max-width:480px){

    .mainHead{
        padding:15px;
    }

    .messHead{
        flex-direction:column;
        gap:15px;
    }

    .logo{
        text-align:center;
        font-size:18px;
    }

    .menu{
        width:100%;

        justify-content:center;

        gap:12px;
    }

    .menu a{
        font-size:15px;
    }

    main{
        margin-top:170px;
        padding:12px;
    }

    .principal{
        width:100%;
        padding:20px;
    }

    h1{
        font-size:2rem;
        line-height:1.2;
    }

    h2{
        font-size:1.5rem;
        line-height:1.3;
    }

    h3{
        font-size:1.05rem;
        line-height:1.4;
    }

    p{
        font-size:1rem;
        line-height:1.7;
    }

    .sobre p{
        font-size:1rem;
    }

    .cards{
        grid-template-columns:1fr;
        gap:20px;
    }

    .card{
        padding:18px;
    }

    .card p{
        font-size:1rem;
    }

    .card img{
        aspect-ratio:16/10;
    }

    .see{
        font-size:1rem;
        padding:13px 20px;
    }

    .tech-card{
        justify-content:flex-start;
    }

    .tech-card div{
        min-width:90px;
        font-size:.9rem;
    }

    .botoes{
        flex-direction:column;
    }

    .botoes button{
        width:100%;
        flex:1 1 auto;
        font-size:1rem;
    }

    .contato{
        flex-direction:column;
    }

    .contato button{
        width:100%;
        flex:1 1 auto;
    }

    .nv{
        flex-direction:column;
        text-align:center;
    }

    .message{
        padding:15px;
    }

    .message div{
        width:100%;
        max-width:420px;
    }
}

@media (max-width:350px){

    .mainHead{
        padding:13px;
        /* font-size: 18px; */
    }

    .logo{
        font-size:17px;
    }

    .menu{
        gap:10px;
    }

    .menu a{
        font-size:14px;
    }

    main{
        margin-top:175px;
        padding:10px;
    }

    .principal{
        padding:16px;
    }

    h1{
        font-size:1.8rem;
    }

    h2{
        font-size:1.4rem;
    }

    h3{
        font-size:1rem;
    }

    p{
        font-size:.95rem;
    }

    .card{
        padding:15px;
    }

    .card p{
        font-size:.95rem;
    }

    .tech-card div{
        min-width:80px;
        font-size:.85rem;
    }
}

      </style>
      
    </head>

    <body class="">

          <!-- HEADER -->
          <header class="mainHead">
          <div class="logo">DEBY 007</div>
          <nav class="menu">
               <a href="#">Home</a>
               <a href="#projetos" onclick="projects()">Projetos</a>
               <a href="#contato">Contato</a>
               <span class="modo" onclick="modo()">🌙</span>
          </nav>
          </header>

          <!-- MAIN -->
          <main>


          <section class="ms">
              <div class="message" id="message">
                   <div class="campo">
                    <header class="messHead">
                        <h2>Send a Message</h2><button onclick="fecharMessage()">X</button>
                    </header>
                        <form id="form">
                            <input type="text" placeholder="Your Name..." id="name" required="">
                            <input type="email" placeholder="Your E-mail..." id="email" required="">
                            <input type="text" placeholder="Send a message..." id="message" required="">
                            <button type="button" id="sendBtn">Send</button>
                        </form>
                   </div>
            </div>
        </section>
          <section class="principal">

               <nav class="nv"><nav><h1 class="nome">EFRAIM JOÃO MANUEL BERNARDO</h1></nav><img alt="efraim.jpg" src="eu.jpg"></nav>
               <h3 class="dev">I am a  <mark>Web DEV Junior </mark></h3>

               <a href="https://github.com/EfraimBernardo" target="_blank"><button class="see" style="background: rgb(23, 30, 40);">See Projects</button></a>

               <!-- SOBRE -->
               <div class="sobre">
               <h2>About me</h2>
               <p>
                    Hey, my name is Efraim Bernardo, and I'm a <strong>Web Developer Junior</strong>.  
                    Welcome to my digital space!

                    I'm passionate about building clean, responsive, and user-friendly websites. My journey into web development began with curiosity and turned into a deep commitment to                             learning and creating. I work mainly with HTML, CSS, JavaScript, and frameworks like React, always striving to grow and improve every day.

                    This portfolio reflects my academic path, personal projects, and the skills I’ve been developing. I believe that code isn't just about functionality — it's also about                             creating experiences. Whether it’s a landing page, a portfolio, or a full web app, I aim to deliver work that is both meaningful and effective.

                    Feel free to explore, check out some of my work, and don’t hesitate to reach out if you'd like to collaborate or just say hi!
               </p><br><br>

              <h2>Techs</h2><br><br>
               <div class="tech-card">
                   <div>HTML</div>
                   <div>CSS</div>
                   <div>JavaScript</div>
                   <div>NodeJS</div>
                   <div>PostgreSQL</div>
                   <div>React.js</div>
                   <div>.Git</div>
                   <div>GitHub</div>
               </div><br><br>

               <!-- PROJETOS -->
               <div class="projetos" id="projetos">
               <h2>Projects</h2>


               <div class="cards">

                    <div class="card">
                    <h3>ARS</h3>
                    <p>Anonymous Reporting System.</p>
                    <img src="Screenshot 2025-12-10 1.36.14 AM.png" alt="Anonymous Reporting System">
                     <a href="https://debygalery.onrender.com/" target="_blank">See on GitHub</a>
                    </div>

                    <div class="card">
                    <h3>LFMS</h3>
                    <p>A Lost and Founds Managemant System.</p>
                    <img src="Screenshot 2025-12-10 1.33.30 AM.png" alt="Lost and Founds Managemant System">
                     <a href="https://debygalery.onrender.com/" target="_blank">See on GitHub</a>
                    </div>

                    <div class="card">
                    <h3>Images Downloader</h3>
                    <p>Web Sie to Download Images</p>
                    <img src="image.png" alt="Lost and Founds Managemant System">
                    <a href="https://debygalery.onrender.com/" target="_blank">See Project</a><br> <a href="https://github.com/EfraimBernardo/Imagens.git" target="_blank">See on GitHub</a>
                    </div>


                   <div class="card">
                    <h3>SIS<strong>TOCKE</strong></h3>
                    <p>Stock Manegement System</p>
                    <img src="stoke.png" alt="Stock Manegement System">
                     <a href="https://github.com/FidelMaluto/sistoke" target="_blank">See on GitHub</a>
                    </div>


                   <div class="card">
                    <h3>User Cadastre</h3>
                    <p>User Cadastre</p>
                    <img src="user.png" alt="User Cadastre">
                     <a href="https://github.com/EfraimBernardo/Userss" target="_blank">See on GitHub</a>
                    </div>


                   <div class="card">
                    <h3>Contact List</h3>
                    <p>Contact List</p>
                    <img src="cont.png" alt="Contact List">
                     <a href="https://github.com/EfraimBernardo/Contactos" target="_blank">See on GitHub</a>
                    </div>

                   <div class="card">
                    <h3>New Student Selection System</h3>
                    <p>For Instituicion</p>
                    <img src="ssne.png" alt="ssne">
                     <a href="https://github.com/EfraimBernardo/SSNE.git" target="_blank">See on GitHub</a>
                    </div>

                   <div class="card">
                    <h3>SkyBank</h3>
                    <p>Digital Wallet & Economy</p>
                    <img src="sky.png" alt="dwe">
                     <a href="https://github.com/EfraimBernardo/SkyBankEconomic.git" target="_blank">See on GitHub</a>
                    </div>

                   <div class="card">
                    <h3>Lissandra Confectionary</h3>
                    <p>Sweets Tenptations</p>
                    <img src="confeitaria.png" alt="lissandra">
                    <a href="https://lissandradocestentacoes.vercel.app/" target="_blank">See Project</a><br> <a href="https://github.com/FidelMaluto/confeitaria-lissandra" target="_blank">See on GitHub</a>
                    </div>

                   <div class="card">
                    <h3>Employees</h3>
                    <p>Employee Management</p>
                    <img src="funcionarios.png" alt="lissandra">
                     <a href="https://github.com/EfraimBernardo/Funcionarios.git" target="_blank">See on GitHub</a>
                    </div>

                   <div class="card">
                    <h3>FEST Chat</h3>
                    <p>Chat App</p>
                    <img src="chat.png" alt="lissandra">
                    <a href="https://debychat.onrender.com/" target="_blank">See Project</a><br> <a href="https://github.com/fe-services-technologies/BatePapo" target="_blank">See on GitHub</a>
                    </div>

                   <div class="card">
                    <h3>NewLys || E-Commerce</h3>
                    <p>E-Commerce</p>
                    <img src="newlys.png" alt="NewLys">
                    <a href="https://newlys-9h0n.onrender.com/.com/" target="_blank">See Project</a><br> <a href="https://github.com/fe-services-technologies/NewLys" target="_blank">See on GitHub</a>
                    </div>
               </div>
               </div>
                   <br><br>

               <!-- CONTATO -->
                   <h2>Contacts</h2>
               <div class="contato" id="contato">
                   <button onclick="sendMessage()">Send me a Message</button>
                <button><a style="text-decoration:none; color: white;" href="https://www.linkedin.com/in/efraim-b-150897352" target="_blank">Here me</a></button>
               <li><a href="https:/wa.me/244938134817" target="_blank"><i class="fab fa-whatsapp"></i></a></li>
               <li><a href="https://github.com/EfraimBernardo" target="_blank"><i class="fab fa-github"></i></a></li>
               <li><a href="https://www.linkedin.com/in/efraim-b-150897352" target="_blank"><i class="fab fa-linkedin"></i></a></li>
               </div>

          </section>

          </main>




<script>
     function sendMessage(){
          const message = document.querySelector(".message");
          message.classList.toggle("send");
     }

    function fecharMessage(){
        const message = document.querySelector(".message");
        message.classList.toggle("close");
    }
    
     function modo(){
          const bd = document.querySelector("body");
          bd.classList.toggle("claro");
     }
    
document.addEventListener("DOMContentLoaded", function() {

    // Inicializa EmailJS
    emailjs.init("oD3WQjnViu0bn4MuP");

    // Pega o botão enviar
    const sendBtn = document.getElementById("sendBtn");

    sendBtn.addEventListener("click", function(e) {
        e.preventDefault(); // previne recarregar

        // Pega os valores do formulário
        const fromName = document.getElementById("name").value;
        const message = document.getElementById("message").value;
        const replyTo = document.getElementById("email").value;

        // Validação básica
        if (!fromName || !message || !replyTo) {
            alert("Por favor, preencha todos os campos!");
            return;
        }

        // Envia o email
        emailjs.send("service_w2m503g", "template_o9f8er6", {
            from_name: fromName,
            message: message,
            reply_to: replyTo
        }).then(function() {
            alert("Mensagem enviada com sucesso!");
        }, function(error) {
            alert("Erro ao enviar mensagem!");
            console.log("EmailJS error:", error);
        });
    });

});
</script>
</body>
    
</html>
