![image](https://github.com/user-attachments/assets/90926c58-ba83-4aa9-9b34-30ece9a33cac)

Gerador de Roteiros para Vídeos do YouTube com IA Gemini

Uma das grandes dificuldades para quem está iniciando um canal no YouTube é justamente a criação de roteiros para os vídeos. O roteiro é uma ferramenta essencial nas produções audiovisuais,
incluindo o YouTube. Então, para ajudar quem tem essa dificuldade, adaptei o código criado na Aula 5 da imersão para criar esta ferramenta, que espero ser de grande ajuda para produtores de conteúdo
para YouTube.

Quero deixar claro que não sou desenvolvedor, por isso optei por fazer as adaptações e ajustes em um código já pronto que, como eu disse anteriormente, foi criado na Aula 5 da imersão.

Minha ideia agora é estudar uma forma de fazer com que esta ferramenta seja migrada para o ambiente Web e, assim, ser acessível para que qualquer pessoa possa utilizá-la. Ainda não sei como fazer isso, mas vou descobrir! 😉

Gostaria de agradecer a todos os envolvidos na Imersão Alura + Google Gemini. Aprendi muito nesses últimos dias e, com certeza, utilizarei muito deste conhecimento adquirido na minha vida pessoal e profissional.

VALEU D+ ❤️

⚠️ A descrição abaixo foi gerada pelo Google Gemini 2.5 Pro (preview) a partir da leitura do arquivo com o código da aplicação em Python (.py):

--------

Este projeto utiliza o poder da IA Generativa do Google, especificamente o modelo Gemini, para criar um sistema de agentes inteligentes capazes de gerar roteiros completos para vídeos do YouTube. 
A partir de um tema fornecido pelo usuário, os agentes colaboram para pesquisar, planejar, redigir e revisar o conteúdo, entregando um roteiro pronto para gravação.

✨ Funcionalidades
Geração Automatizada de Roteiros: Crie roteiros para vídeos do YouTube de forma rápida e eficiente.
Sistema Multiagente:
Agente Buscador: Pesquisa notícias e conteúdos recentes e de alto impacto sobre o tema especificado, respeitando as diretrizes do YouTube.
Agente Planejador: Analisa os conteúdos buscados, identifica os pontos cruciais e define a estrutura do roteiro, selecionando o tema de maior relevância.
Agente Redator: Transforma o plano de conteúdo em um rascunho de roteiro envolvente, educativo, de fácil compreensão e com duração mínima de 10 minutos. Também sugere títulos, conceitos de thumbnails e descrições otimizadas para SEO.
Agente Revisor: Atua como editor, refinando o rascunho do roteiro, verificando clareza, concisão, correção gramatical e factual, e adequação ao tom desejado.
Baseado em Pesquisa Atual: Os roteiros são gerados com base em informações recentes coletadas em tempo real.
Otimização para YouTube: Inclui sugestões de títulos, thumbnails e descrições focadas em SEO.
Fácil de Usar: Basta fornecer o tema do vídeo para iniciar o processo.

⚙️ Como Funciona
O sistema opera através de uma sequência de agentes especializados:

Entrada do Usuário: O usuário fornece o tema desejado para o vídeo do YouTube.
Agente Buscador: O primeiro agente (agente_buscador) realiza uma pesquisa no Google para encontrar as notícias e conteúdos mais atuais e relevantes sobre o tema, considerando um período recente (último mês).
Agente Planejador: O agente_planejador recebe os resultados da busca e, utilizando o Google Search novamente, aprofunda-se nos itens para determinar os pontos cruciais a serem cobertos. 
Ele seleciona o tema de maior relevância e define uma estrutura para o roteiro.
Agente Redator: Com o plano definido, o agente_redator elabora um rascunho completo do roteiro. Este rascunho é projetado para ser envolvente, educativo e ter uma duração mínima de 10 minutos. 
Além disso, o agente sugere títulos otimizados para SEO, ideias para thumbnails e uma descrição para o vídeo.
Agente Revisor: Por fim, o agente_revisor analisa o rascunho do roteiro, verificando a clareza, correção (gramatical e factual) e a adequação ao público-alvo. Ele pode aprovar o roteiro ou sugerir melhorias.
Saída: O sistema apresenta o roteiro finalizado e a revisão do mesmo.

📋 Pré-requisitos
Antes de executar o projeto, você precisará ter:

Python instalado.
Uma chave de API do Google Gemini.

🚀 Instalação e Configuração
Clone o repositório (se aplicável) ou baixe o arquivo Python.

Instale as dependências:
O script utiliza as seguintes bibliotecas Python, que podem ser instaladas via pip:

Bash

pip install google-genai google-adk requests
O script original contém %pip -q install google-genai e !pip install -q google-adk para ambientes como o Google Colab.

Configure a Chave da API do Google Gemini:
O script espera que a chave da API do Google Gemini esteja configurada como uma variável de ambiente ou através do sistema userdata do Google Colab.
Para configurar como variável de ambiente localmente:

Bash

export GOOGLE_API_KEY="SUA_CHAVE_API_AQUI"
Ou modifique a linha no código para inserir sua chave diretamente (não recomendado para compartilhamento público):

Python

os.environ["GOOGLE_API_KEY"] = "SUA_CHAVE_API_AQUI"

▶️ Como Usar
Execute o script Python:

Bash

python nome_do_arquivo.py
(Substitua nome_do_arquivo.py pelo nome real do arquivo, por exemplo, gerador_de_roteiros_para_vídeos_do_youtube_imersão_ia_alura_+_google_gemini.py).

Quando solicitado, digite o tema do seu vídeo para o YouTube:

▶️ Por favor, digite o tema do seu vídeo para o YouTube: [Seu Tema Aqui]
Aguarde o processamento. O script passará pelas etapas de busca, planejamento, redação e revisão, exibindo mensagens de progresso.

Ao final, o roteiro gerado e a revisão serão exibidos.

🤝 Contribuições
Contribuições são bem-vindas! Se você tiver ideias para melhorias, novas funcionalidades ou correções de bugs, sinta-se à vontade para:

Fazer um "fork" do projeto.
Criar uma nova "branch" (git checkout -b feature/nova-feature).
Fazer "commit" de suas alterações (git commit -am 'Adiciona nova feature').
Fazer "push" para a "branch" (git push origin feature/nova-feature).
Abrir um "Pull Request".
