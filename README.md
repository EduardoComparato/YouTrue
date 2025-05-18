# YouTrue
<img src="https://github.com/user-attachments/assets/d1c5e3cb-a532-4730-8ad2-30e805986608" height="150">

**YouTrue** é um sistema multi-agentes de verificação de informações projetado para analisar e validar o conteúdo de vídeos do YouTube e textos brutos. Utilizando uma arquitetura baseada em agentes, o sistema transcreve vídeos, revisa o texto, busca fontes relevantes e aponta possíveis erros ou inconsistências, indicando graus de confiabilidade.

## Linguagem utilizada
<img src="https://static.wixstatic.com/media/efe4c3_6865853cc59c4bc89ef3191bba086130~mv2.jpg/v1/fill/w_560,h_188,al_c,q_80,usm_0.66_1.00_0.01,enc_auto/efe4c3_6865853cc59c4bc89ef3191bba086130~mv2.jpg" height="20">

# Objetivo
Auxiliar na verificação de confiabilidade de conteúdos no YouTube e textos brutos, detectando desinfomação, uso de fake news ou afins, e incongruências, tendo relevância acadêmica, científica e social.
___
# Requisitos
- Google Colab
- Python 3 (ao executar fora do Google Colab)
- Bibliotecas `google-genai`, `google-adk`, `youtube-transcript-api` (todas instaladas através do código, **se executado no Google Colab**)
- Chaves de API do Google Gemini


# Funcionalidades
- **📄Transcrição de Vídeos**
> Transcreve automaticamente o áudio de vídeos do YouTube para análise textual. Aceita transcrições que venham das línguas português (pt-BR e pt), inglês (en-US e en) e espanhol (es).
- **✒️Revisão de Texto**
> Revisa e formata o texto transcrito, removendo elementos de minutagem e tópicos, e traduzindo para o português, se necessário.
- **🕵️Busca de Fontes**
> Busca em múltiplas fontes confiáveis informações relevantes ao tema do vídeo para comparação.
- **👁️Apontamento de Erros**
> Compara o texto do vídeo com as fontes encontradas, identifica erros e fornece correções com base em evidências.
- **👍Avaliação de Confiabilidade**
> Atribui um grau de confiabilidade ao conteúdo do vídeo original com base na quantidade de erros encontrados.

# Instruções

### Passo 1: Tipo
Indique se o conteúdo indicado é um texto ou um ID, sendo que:
- 1 - ID
- 2 - Texto

### Passo 1.1: ID
Caso tenha selecionado a 1° opção, deve ser fornecido o ID, não o URL. A seguir, exemplos de onde se encontra o ID, a partir da URL:

#### URL "youtube.com"
- Link exemplo: https://www.youtube.com/watch?v=dQw4w9WgXcQ
  - O ID é o que se encontra após o "v=", no caso, dQw4w9WgXcQ

#### URL "youtu.be"
- Link exemplo: https://youtu.be/dQw4w9WgXcQ?si=KQ9WdBWFJ97sI_QK
  - O ID é o que se encontra entre ".be/" e "?si", no caso, dQw4w9WgXcQ

> [!WARNING]
>
> Em caso de erro no 1° agente, tente fornecer o ID novamente ou reinicie a página.

> [!TIP]
>
> Para um melhor aproveitamento, forneça vídeos e textos com conteúdos que seja possível a investigação por pesquisa. 

# Limitações
- A precisão da transcrição pode variar dependendo da qualidade do áudio do vídeo
- A disponibilidade de transcrições pode variar dependendo das configurações do vídeo no YouTube
- O sistema se concentra em fontes textuais e pode não ser adequado para analisar conteúdo altamente visual
___
# FAQ

### Q: Como posso executar o código por outra IDE ou plataforma externa além do Google Colab?

Por ser necessário a instalação de bibliotecas do Google, recomenda-se a execução no Google Colab para maior facilidade.
Caso deseje executar em outro local, provavelmente será necessária a instalação do Python 3.x. Cada IDE e plataforma funciona de maneira diferente, então deverá verificar como instalar cada biblioteca utilizada no código na plataforma/IDE que for executar.

# Créditos
Gostaria de dar os créditos a Alura e principalmente todos os envolvidos na Imersão IA Alura + Google Gemini de 2025, contexto para o qual este projeto foi desenvolvido. Agradeço aos hosts Fabrício Carraro, Luciano Martins e Valquíria Alencar, assim como a comunidade do Discord feita para a imersão, onde pude trocar ideias, sugestões, conselhos e apoios.

# Contribuições
Contribuições para o projeto são bem-vindas 😁! Se você tiver
- **Sugestões de melhoria**;
- **Correções de bugs**;
- **Novas funcionalidades**,
sinta-se à vontade para abrir uma issue ou enviar um pull request.
