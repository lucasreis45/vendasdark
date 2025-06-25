<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Oferta Exclusiva - O Caminho para Sua Primeira Venda</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        :root {
            --cor-preto: #0a0a0a;
            --cor-dourado: #FFD700;
            --cor-dourado-escuro: #B8860B;
            --cor-texto: #EAEAEA;
            --cor-fundo-secao: #181818;
        }

        /* Animações de Scroll */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .animate-on-scroll {
            animation: fadeIn 1s ease-out forwards;
            animation-play-state: paused;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--cor-preto);
            color: var(--cor-texto);
            margin: 0;
            padding: 0;
            text-align: center;
        }
        
        /* BANNER DE TOPO */
        .top-banner {
            background-color: var(--cor-dourado);
            color: var(--cor-preto);
            padding: 10px 20px;
            font-weight: 700;
            font-size: 0.9rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            width: 100%;
            box-sizing: border-box;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }

        .header {
            padding: 60px 20px 40px 20px;
        }

        .header h1 {
            font-size: 2.8rem;
            font-weight: 900;
            color: var(--cor-dourado);
            line-height: 1.2;
            margin-bottom: 15px;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.3);
        }

        .header p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto;
        }

        .section {
            padding: 40px 20px;
            margin-bottom: 20px;
        }

        .subheadline ul {
            list-style: none;
            padding: 0;
            max-width: 500px;
            margin: 20px auto;
        }

        .subheadline li {
            background-color: var(--cor-fundo-secao);
            border-left: 4px solid var(--cor-dourado);
            padding: 15px 20px;
            margin-bottom: 10px;
            text-align: left;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .subheadline .icon {
            stroke: var(--cor-dourado);
            flex-shrink: 0;
        }

        .pain-section h2 {
            font-size: 2rem;
            color: var(--cor-dourado);
            max-width: 600px;
            margin: 0 auto 20px auto;
        }
        
        .product-presentation {
            display: flex;
            align-items: center;
            gap: 40px;
            background-color: var(--cor-fundo-secao);
            padding: 40px;
            border-radius: 12px;
            text-align: left;
        }

        .product-image img {
            max-width: 280px;
            width: 100%;
            border-radius: 8px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.7);
            transition: transform 0.3s ease;
        }
        
        .product-image img:hover {
            transform: scale(1.05) rotateZ(-2deg);
        }

        .product-benefits ul { list-style: none; padding: 0; }
        
        .product-benefits li {
            font-size: 1.1rem;
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
            gap: 10px;
        }
        .product-benefits .icon {
            stroke: var(--cor-dourado);
            margin-top: 4px;
            flex-shrink: 0;
        }

        /* ESTILOS DA NOVA PROVA SOCIAL */
        .testimonials { padding: 30px 0; }

        .testimonials h2 {
            margin-bottom: 40px;
        }

        .testimonial-message {
            background-color: var(--cor-fundo-secao);
            border: 1px solid #282828;
            max-width: 550px;
            margin: 25px auto;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.5);
            text-align: left;
        }
        
        .testimonial-header {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 15px 20px;
            border-bottom: 1px solid #282828;
        }

        .avatar {
            width: 45px;
            height: 45px;
            border-radius: 50%;
            background-color: var(--cor-dourado-escuro);
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            font-size: 1.2rem;
            color: var(--cor-preto);
        }

        .user-info .name {
            font-weight: 700;
            color: var(--cor-texto);
        }

        .user-info .location {
            font-size: 0.8rem;
            color: #999;
        }
        
        .testimonial-body {
            padding: 20px;
            font-size: 1.05rem;
            line-height: 1.6;
        }

        .testimonial-body p {
            margin: 0 0 15px 0;
        }

        .testimonial-body .timestamp {
            font-size: 0.8rem;
            color: #777;
            text-align: right;
        }
        

        .offer-box {
            background-color: var(--cor-preto);
            border: 2px solid var(--cor-dourado);
            border-radius: 10px;
            padding: 40px;
            box-shadow: 0 0 25px rgba(255, 215, 0, 0.25);
        }
        
        .offer-box .price-old { font-size: 1.2rem; text-decoration: line-through; opacity: 0.7; }

        .offer-box .price-new {
            font-size: 3.5rem;
            font-weight: 900;
            color: var(--cor-dourado);
            margin: 10px 0;
        }
        
        .offer-box .price-details { font-size: 1rem; }

        .bonus-box { margin-top: 30px; padding: 20px; border-top: 1px solid var(--cor-dourado-escuro); }
        
        .bonus-box h3 { color: var(--cor-dourado); }
        
        .bonus-box ul { list-style: none; padding: 0; text-align: left; max-width: 400px; margin: auto; }
        .bonus-box li { display: flex; align-items: flex-start; gap: 10px; margin-bottom: 10px; }

        .cta-button {
            display: inline-block;
            background: linear-gradient(145deg, var(--cor-dourado), var(--cor-dourado-escuro));
            color: var(--cor-preto);
            padding: 20px 40px;
            font-size: 1.5rem;
            font-weight: 900;
            text-decoration: none;
            border-radius: 8px;
            margin: 20px 0;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2), 0 0 20px rgba(255, 215, 0, 0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .cta-button:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.4), 0 0 30px rgba(255, 215, 0, 0.5);
        }
        
        .cta-button-small { font-size: 1.2rem; padding: 15px 30px; }

        .security-lock { margin-top: 30px; font-weight: bold; display: flex; align-items: center; justify-content: center; gap: 8px;}
        
        .final-message { margin-top: 40px; padding-top: 20px; border-top: 1px solid #333; }
        
        .final-message p { font-style: italic; max-width: 600px; margin: 15px auto; }

        .countdown-timer { margin: 40px 0 20px 0; padding-top: 30px; border-top: 1px dashed var(--cor-dourado-escuro); }

        .countdown-timer h3 {
            color: var(--cor-texto);
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        .timer-display { display: flex; justify-content: center; gap: 15px; }

        .timer-display div {
            display: flex;
            flex-direction: column;
            background: var(--cor-fundo-secao);
            padding: 10px;
            border-radius: 5px;
            min-width: 70px;
        }

        .timer-display span { font-size: 2.5rem; font-weight: 900; color: var(--cor-dourado); }
        
        .timer-display .label { font-size: 0.7rem; text-transform: uppercase; color: #aaa; margin-top: 5px; }
        
        @media (max-width: 768px) {
            .header h1 { font-size: 2.2rem; }
            .product-presentation { flex-direction: column; text-align: center; }
            .product-benefits { text-align: left; margin-top: 20px; }
            .timer-display { gap: 8px; }
            .timer-display div { min-width: 60px; }
            .timer-display span { font-size: 2rem; }
        }
    </style>
</head>
<body>

    <!-- Banner de Topo Editável -->
    <div class="top-banner">
        <span>Atenção: Oferta e Bônus Exclusivos por Tempo Limitado!</span>
    </div>

    <div class="container">

        <header class="header animate-on-scroll">
            <h1>🔥 Seu salário acaba antes do fim do mês? E se o seu celular pudesse pagar suas contas?</h1>
            <p>Descubra o método validado para fazer suas primeiras vendas online, <strong>usando apenas o celular</strong>, sem precisar aparecer e sem gastar 1 real com anúncios.</p>
        </header>

        <section class="section subheadline animate-on-scroll">
            <h2>Atenção: Isto não é mais um "curso"...</h2>
            <ul>
                <li>
                    <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>
                    <span>NÃO precisa ter seguidores (o método funciona do zero).</span>
                </li>
                <li>
                    <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>
                    <span>NÃO precisa fazer dancinhas (venda 100% no anonimato).</span>
                </li>
                <li>
                    <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>
                    <span>NÃO precisa investir em tráfego pago (o jogo aqui é 100% orgânico).</span>
                </li>
            </ul>
        </section>

        <section class="section pain-section animate-on-scroll">
            <h2>🚨 Seja honesto: dói ver gente comum faturando no Instagram e TikTok enquanto sua conta bancária continua a mesma, certo?</h2>
            <p>Enquanto você apenas consome conteúdo, outros estão transformando seguidores em dinheiro. Este Mini Ebook é o atalho que você precisava para parar de ser espectador e <strong>finalmente entrar no jogo.</strong></p>
        </section>

        <section class="section product-presentation animate-on-scroll">
            <div class="product-image">
                <img src="https://i.postimg.cc/GpPgsndj/19-90-1.png" alt="Oferta Especial Ebook por R$19,90">
            </div>
            <div class="product-benefits">
                <h2>✅ O Que Você Terá em Mãos:</h2>
                <ul>
                    <li>
                        <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"></path></svg>
                        <strong>Criar Conteúdos Magnéticos:</strong> Aprenda a estrutura de posts e vídeos que fazem as pessoas pararem de rolar o feed e te chamar no privado.
                    </li>
                    <li>
                        <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"></path></svg>
                        <strong>Scripts de Venda Prontos:</strong> O "copia e cola" exato para conversar com clientes no Direct e WhatsApp e conduzir a conversa para o PIX.
                    </li>
                    <li>
                        <svg class="icon" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"></path></svg>
                        <strong>Transformar Views em Vendas:</strong> Descubra como vídeos simples se tornam uma máquina de gerar mensagens de pessoas querendo comprar.
                    </li>
                </ul>
            </div>
        </section>
        
        <section class="section testimonials animate-on-scroll">
             <h2>📲 O que dizem os nossos alunos:</h2>
            
            <div class="testimonial-message">
                <div class="testimonial-header">
                    <div class="avatar">MS</div>
                    <div class="user-info">
                        <div class="name">Mariana S.</div>
                        <div class="location">Sorocaba, SP</div>
                    </div>
                </div>
                <div class="testimonial-body">
                    <p>Gente, sério, eu NUNCA tinha vendido NADA online. Achei que não ia rolar pra mim. Comprei o guia ontem sem botar muita fé... apliquei a dica do vídeo de 7s e fiz minha primeira venda de R$47 hoje! Tô em choque kkkkk</p>
                    <div class="timestamp">Hoje 14:31</div>
                </div>
            </div>

            <div class="testimonial-message">
                <div class="testimonial-header">
                    <div class="avatar">JV</div>
                    <div class="user-info">
                        <div class="name">João Victor</div>
                        <div class="location">@joaovictor.mkt</div>
                    </div>
                </div>
                <div class="testimonial-body">
                    <p>Cara, só pra agradecer. Tava patinando há meses, gastando com anúncio que não dava em nada. O checklist diário de vocês me salvou. Consegui R$189,90 no orgânico só nesse fds. Vlw mesmo!</p>
                    <div class="timestamp">Enviado ontem</div>
                </div>
            </div>
        </section>

        <section class="section offer-box animate-on-scroll">
            <h2>💎 Por que este material tem um valor?</h2>
            <p>Porque ele te economiza tempo e dinheiro. Ele vai direto ao ponto, sem enrolação. E o principal: <strong>quem paga, se compromete. Quem se compromete, vende.</strong></p>
            <hr style="border: 0; height: 1px; background-image: linear-gradient(to right, rgba(0, 0, 0, 0), var(--cor-dourado-escuro), rgba(0, 0, 0, 0)); margin: 30px 0;">
            <h2>🎯 OFERTA DE LANÇAMENTO</h2>
            <p>O preço vai subir! Garanta agora seu acesso imediato com valor promocional:</p>
            <p class="price-old">De: <del>R$49,90</del></p>
            <p class="price-new">POR APENAS: R$ 19,90</p>
            <p class="price-details">(Menos de R$0,67 por dia no mês para aprender a fazer R$50, R$100 ou mais por dia)</p>

            <div class="bonus-box">
                <h3>🎁 BÔNUS ESPECIAL (SÓ HOJE)</h3>
                 <ul>
                    <li><svg class="icon" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg> <span>Acesso ao Grupo de Alunos no WhatsApp.</span></li>
                    <li><svg class="icon" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="4" y1="9" x2="20" y2="9"></line><line x1="4" y1="15" x2="20" y2="15"></line><line x1="10" y1="3" x2="8" y2="21"></line><line x1="16" y1="3" x2="14" y2="21"></line></svg> <span>Lista Secreta de Hashtags Virais.</span></li>
                    <li><svg class="icon" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M13 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V9z"></path><polyline points="13 2 13 9 20 9"></polyline></svg> <span>Checklist Diário de Ações que Geram Vendas.</span></li>
                </ul>
            </div>
            
            <div id="countdown" class="countdown-timer">
                <h3>Esta oferta termina em:</h3>
                <div class="timer-display">
                    <div><span id="hours">00</span><div class="label">Horas</div></div>
                    <div><span id="minutes">00</span><div class="label">Minutos</div></div>
                    <div><span id="seconds">00</span><div class="label">Segundos</div></div>
                </div>
            </div>

            <a href="https://pay.cakto.com.br/rxip6ud_447660" class="cta-button">👉 QUERO MEU EBOOK E TODOS OS BÔNUS AGORA! 👈</a>
            <p class="security-lock">
                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>
                <span>Compra 100% Segura e Acesso Imediato</span>
            </p>
        </section>

        <section class="section final-message animate-on-scroll">
             <h2>📌 Um recado final, de quem já esteve no seu lugar...</h2>
             <p>"Eu sei o que é o medo de tentar e se frustrar de novo. Mas a verdade é uma só: se você não der um passo diferente, sua realidade financeira continuará exatamente a mesma."</p>
             <p>Esta é a chance mais direta e barata que você vai encontrar. Tome a decisão que o "Você do Futuro" vai te agradecer.</p>
             <a href="https://pay.cakto.com.br/rxip6ud_447660" class="cta-button cta-button-small">✅ Sim, eu decido começar agora!</a>
        </section>
        
    </div>

    <script>
    document.addEventListener("DOMContentLoaded", function() {
        // Lógica do cronômetro
        (function() {
            const countdownDuration = 24 * 60 * 60 * 1000;
            let countDownDate = localStorage.getItem('countDownDate_v3');
            if (!countDownDate || new Date().getTime() > parseInt(countDownDate, 10)) {
                countDownDate = new Date().getTime() + countdownDuration;
                localStorage.setItem('countDownDate_v3', countDownDate);
            } else {
                countDownDate = parseInt(countDownDate, 10);
            }

            const x = setInterval(function() {
                const now = new Date().getTime();
                const distance = countDownDate - now;

                if (distance < 0) {
                    clearInterval(x);
                    document.getElementById("countdown").innerHTML = "<h3 style='color: var(--cor-dourado);'>OFERTA ENCERRADA!</h3>";
                    return;
                }
                
                const hours = Math.floor(distance / (1000 * 60 * 60));
                const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((distance % (1000 * 60)) / 1000);

                const formatTime = (time) => String(time).padStart(2, '0');

                document.getElementById("hours").innerText = formatTime(hours);
                document.getElementById("minutes").innerText = formatTime(minutes);
                document.getElementById("seconds").innerText = formatTime(seconds);

            }, 1000);
        })();

        // Lógica de animação ao rolar
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animationPlayState = 'running';
                    observer.unobserve(entry.target);
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.animate-on-scroll').forEach(section => {
            observer.observe(section);
        });
    });
    </script>

</body>
</html>
