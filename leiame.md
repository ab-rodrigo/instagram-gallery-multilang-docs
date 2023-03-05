## Instagram Gallery Multi-language - OpenCart v3.x (OCMOD)

![Badge](https://img.shields.io/badge/oc_version-3.x-informational?style=flat&logoColor=white)
![Badge](https://img.shields.io/badge/ocmod-true-informational?style=flat&logoColor=white)
[![Badge](https://img.shields.io/badge/donate--brightgreen?style=flat&logoColor=white&logo=paypal)](https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW)

### <img src="images/external_link_icon.png" width="30" alt="Module page" title="Module page"><a href="https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=44767&filter_member=Rodrigoabr" target="_blank"> Module page</a>

- [Bem-vindo](#bem-vindo)
- [Visão geral](#visão-geral)
- [Recursos](#recursos)
- [Pré-requisitos](#pré-requisitos)
- [Carregar arquivos](#carregar-arquivos)
- [Instalar o módulo](#instalar-o-módulo)
- [Galerias](#galerias)
  - [Criar uma Galeria Principal](#criar-uma-galeria-principal)
  - [Criar uma Galeria Clone](#criar-uma-galeria-clone)
- [Configuração da API (Somente para Galerias Principais )](#configuração-da-api-somente-para-galerias-principais-)
  - [Crie um aplicativo do Facebook](#crie-um-aplicativo-do-facebook)
  - [Módulo de configuração da API e exibição básica do Instagram](#módulo-de-configuração-da-api-e-exibição-básica-do-instagram)
  - [Adicionar um usuário de teste do Instagram](#adicionar-um-usuário-de-teste-do-instagram)
  - [Autenticar o usuário](#autenticar-o-usuário)
- [Aba de configuração geral](#aba-de-configuração-geral)
- [Aba de configuração de visualização](#aba-de-configuração-de-visualização)
- [Exibir a galeria no layout.](#exibir-a-galeria-no-layout)
- [Permissões de acesso e modificação](#permissões-de-acesso-e-modificação)
- [Desinstalar](#desinstalar)
- [Solução de problemas](#solução-de-problemas)
- [Licença](#licença)
- [Como obter ajuda](#como-obter-ajuda)
- [Contato](#contato)
- [Buy me a coffee](#buy-me-a-coffee)

# Bem-vindo
Bem-vindo à documentação do módulo Instagram Gallery Multi-Language para Opencart versões 3.x.

# Visão geral
Exiba suas postagens do Instagram diretamente em sua loja com facilidade. Utilize a API oficial do Meta para exibir suas postagens do Instagram como uma galeria de imagens em sua loja online. Crie uma variedade de visualizações, adicione efeitos, títulos, legendas, links para a postagem de mídia original, botões de navegação, botões de paginação e muito mais. Configure a API uma vez e crie várias galerias, cada uma com um estilo de visualização único e exiba-as em diferentes layouts.
<p align="center"><img src="images/overview.png" alt="Visão geral" title="Visão geral"></p>

# Recursos
+ 3 tipos de visualização
+ Título
+ Legenda
+ Paginação
+ Link para postagem original no Instagram
+ Efeitos de imagem
+ Clone de galeria (Múltiplas galerias com uma única API)
+ Disponível em
   - Inglês (en-gb)
   - Português (pt-br)

# Pré-requisitos
+ OpenCart v3.x instalado como site público com certificado SSL (**o certificado SSL é necessário para a integração da API**).
+ Uma [Conta de Desenvolvedor do Facebook](https://developers.facebook.com/).
+ Uma [conta no Instagram](https://www.instagram.com/).
+ O usuário deve ter as seguintes permissões de acesso e modificação:
  - *Painel > Extensões > Instalador*
  - *Painel > Extensões > Extensões*
  - *Painel > Extensões > Modificações*
  - *Painel > Design > Layout*

Para conceder ou revogar permissões, consulte a seção [Permissões de Acesso e Modificação](#permissões-de-acesso-e-modificação).

# Carregar arquivos
Acesse **_Extensões_ > _Instalador_**. No formulário que aparece, clique no botão **_Carregar_**.
<p align="center"><img src="images/upload_file.png" width="600" alt="Carregar arquivos" title="Carregar arquivos"></p>

Localize o arquivo **instagra_gallery_multilang_3.x.ocmod.zip** que foi baixado anteriormente, selecione-o e clique no botão **_Abrir_** ou dê um duplo clique no nome do arquivo.

<p align="center"><img src="images/select_instalation_file.png" width="600" alt="Selecionar arquivo de instalação" title="Selecionar arquivo de instalação"></p>

Aguarde a instalação ser concluída e o módulo será listado na tabela de **_Histórico de Instalação_**.

Acesse **_Extensões_ > _Modificações_** e clique no botão **_Atualizar_**.
<p align="center"><img src="images/refresh_modifications.png" width="600" alt="Atualizar modificações" title="Atualizar modificações"></p>

# Instalar o módulo
Acesse **_Extensões_ > _Extensões_**, selecione **_Módulos_** no menu suspenso, localize o **_Instagram Gallery Multilang_** e, em seguida, clique no botão **_Instalar_** no final da linha.
<p align="center"><img src="images/install_module.png" width="600" alt="Instalar o módulo" title="Instalar o módulo"></p>

# Galerias
Sobre os tipos de galeria
>Existem duas maneiras de criar uma galeria:
>1. [_Galeria Principal_ ou _Galeria Pai_](#criar-uma-galeria-principal): Este tipo de galeria irá conter a configuração da API do Instagram. Várias Galerias Principais podem ser criadas, cada uma com uma configuração de API diferente.
>2. [_Galeria Clone_ ou _Galeria Filho_](#criar-uma-galeria-clone): Este tipo de galeria usará as configurações de API da Galeria Principal. Várias Galerias Clone também podem ser criadas para cada Galeria Principal.

## Criar uma Galeria Principal
Vá para **_Extensões_ > _Extensões_**, selecione **_Módulos_** no menu suspenso, localize **_Instagram Gallery Multilang_**, e clique no botão **_Editar_** no final da linha.
<p align="center"><img src="images/add_gallery.png" width="600" alt="Adicionar galeria" title="Adicionar galeria"></p>

Digite o nome da _nova galeria_ e clique no botão Salvar. O nome da galeria pode ser alterado posteriormente.
<p align="center"><img src="images/add_gallery_name.png" width="600" alt="Adicionar galeria" title="Adicionar galeria"></p>

## Criar uma Galeria Clone
Vá para **_Extensões_ > _Extensões_**, selecione **_Módulos_** no menu suspenso, localize **_Instagram Gallery Multilang_**, e clique no botão **_Editar_** no final da linha.
<p align="center"><img src="images/add_gallery.png" width="600" alt="Adicionar galeria clone" title="Adicionar galeria clone"></p>

Digite o nome da _nova galeria filho_, selecione a _galeria pai_ e clique no botão Salvar. O nome da galeria pode ser alterado posteriormente.
<p align="center"><img src="images/add_clone_gallery_name.png" width="600" alt="Adicionar nome da galeria clone" title="Adicionar nome da galeria clone"></p>

# Configuração da API (Somente para Galerias Principais )

Este capítulo/tutorial demonstra como configurar um aplicativo do Instagram no painel do aplicativo e como configurar a API para o módulo.

>Antes de começar, certifique-se de que você já possui uma [Conta de Desenvolvedor do Facebook](https://developers.facebook.com/) e que a loja não está em modo de manutenção.

## Crie um aplicativo do Facebook

Acesse a [Conta de Desenvolvedor do Facebook](https://developers.facebook.com/), clique em **_Meus Apps_** e crie um novo aplicativo.

<p align="center"><img src="images/my_apps_empty.png" width="600" alt="Meus aplicativos" title="Meus aplicativos"></p>

Escolha o tipo de aplicativo **_Consumidor_** ou **_Nenhum_**.

<p align="center"><img src="images/app_type.png" width="400" alt="Tipo de aplicativo" title="Tipo de aplicativo"></p>

Adicione um nome de aplicativo.

<p align="center"><img src="images/add_app_name.png" width="600" alt="Adicionar nome do aplicativo" title="Adicionar nome do aplicativo"></p>

Depois de criar o aplicativo, vá para o Painel do aplicativo, navegue até **_Configurações > Básico_**, role até o final da página e clique em **_Adicionar plataforma_**.

<p align="center"><img src="images/add_plataform.png" width="600" alt="Adicionar plataforma" title="Adicionar plataforma"></p>

Escolha **_Website_** e clique em **_Avançar_**.

<p align="center"><img src="images/select_plataform.png" width="400" alt="Selecionar tipo de plataforma" title="Selecionar tipo de plataforma"></p>

Adicione a URL do seu website e salve as alterações.

><img src="images/copy_button.png" width="50" alt="Botão copiar" title="Botão copiar">
>Clique neste botão para copiar a URL da loja.

<p align="center"><img src="images/copy_paste_website_url.png" width="600" alt="Adicionar URL do website" title="Adicionar URL do website"></p>

## Módulo de configuração da API e exibição básica do Instagram
Clique em **_Produtos_**, localize o produto **_Instagram Basic Display_** e clique em **_Configurar_** para adicioná-lo ao seu aplicativo.
<p align="center"><img src="images/instagram_basic_display_setup.png" width="600" alt="Instagram basic display setup" title="Instagram basic display setup"></p>

Role a página para baixo e clique em **_Criar novo aplicativo_**.
<p align="center"><img src="images/create_new_app.png" width="600" alt="Instagram basic display setup" title="Instagram basic display setup"></p>

Digite o nome do aplicativo do Facebook que você acabou de criar.
<p align="center"><img src="images/create_a_new_instagram_app_id.png" width="600" alt="Create a new Instagram App ID" title="Create a new Instagram App ID"></p>

Por favor, volte para a aba API do módulo, copie a URL da loja e cole-a nos campos **_URI de redirecionamento OAuth válida_**, **_URL de retorno de chamada de desautorização_** e **_URL de solicitação de exclusão de dados_**, em seguida, clique em 'Salvar'.
<p align="center"><img src="images/copy_paste_oauth_uri.png" width="600" alt="Copy and paste OAuth URI" title="Copy and paste OAuth URI"></p>

No formulário de Exibição Básica do Instagram, copie os números do **_ID do aplicativo do Instagram_** e do **_segredo do aplicativo do Instagram_** e cole-os na aba API do módulo.
<p align="center"><img src="images/copy_paste_instagram_ids.png" width="600" alt="Copy and paste Instagram App ID" title="Copy and paste Instagram App ID"></p>

## Adicionar um usuário de teste do Instagram
Navegue até **_Funções > Funções_** e role para baixo até a seção **_Adicionar testadores do Instagram_**. Em seguida, clique em **_Adicionar testadores do Instagram_** e digite o nome de usuário da sua conta do Instagram antes de enviar o convite.
<p align="center"><img src="images/add_instagram_test_user.png" width="600" alt="Add Instagram user test" title="Add Instagram user test"></p>

Abra um novo navegador da web e vá para o instagram.com. Faça login na sua conta do Instagram recém-convidada. Navegue até **_(Ícone do perfil) > Editar perfil > Aplicativos e sites > Convites de teste_**, e aceite o convite.
<p align="center"><img src="images/tester_invites.png" width="600" alt="Tester invites" title="Tester invites"></p>

Sua conta do Instagram agora é elegível para ser acessada por meio do seu aplicativo do Facebook.

## Autenticar o usuário
Vá para a aba API do módulo e clique no botão **_Autorização_**.
<p align="center"><img src="images/authorization_button.png" width="600" alt="Botão de Autorização" title="Botão de Autorização"></p>

Clique no botão **_Abrir Janela de Autorização_** ou copie e cole o link em seu navegador. É necessário estar logado na conta do Instagram que fornecerá a mídia para a galeria.
<p align="center"><img src="images/authorization_popup.png" width="400" alt="Janela de Autorização" title="Janela de Autorização"></p>

A janela de autorização deve aparecer e exibir seu nome de usuário do Instagram, o nome do aplicativo e uma descrição das permissões que está solicitando. Clique em **_Autorizar_** para conceder acesso do aplicativo aos dados do seu perfil.
<p align="center"><img src="images/authorization_window.png" width="250" alt="Janela de Autorização" title="Janela de Autorização"></p>

Por favor, acesse a página do módulo e atualize-a. Em seguida, vá para a aba API e verifique se o status da API exibe a mensagem de API configurada correta.
<p align="center"><img src="images/api_status_success.png" width="600" alt="Sucesso da API" title="Sucesso da API"></p>

A configuração para o Instagram Basic Display e a API do módulo está completa quando o status da API exibe a mensagem de API configurada correta. Configure as configurações Gerais e de Visualização e clique no botão 'Salvar' no topo da página para criar sua galeria.

# Aba de configuração geral
<p align="center"><img src="images/general_tab_form.png" width="600" alt="Configuração Geral" title="Configuração Geral"></p>

+ **Nome**: Este texto é usado para identificar a galeria. Nomes duplicados para galerias não são permitidos.
+ **Título**: O título que será exibido acima da galeria permite que você use HTML e CSS.
+ **Tipos de postagens**: Tipos de postagens do Instagram que fornecerão conteúdo para a galeria.
+ **Tipo de mídia do álbum**: Tipos de mídia que serão fornecidos dos álbuns.
+ **Imagens do álbum**: A quantidade de mídia que será fornecida dos álbuns.
+ **Atualização**: Período durante o qual a imagem mais antiga da galeria será atualizada.
+ **Status**: Status da galeria.

# Aba de configuração de visualização
<p align="center"><img src="images/view_tab.png" width="600" alt="Configuração de visualização" title="Configuração de visualização"></p>

+ **Mídia por visualização**: O número máximo de imagens que será exibido.
+ **Tipo de visualização**: Tipo de visualização.
+ **Paginação**: Mostrar pontos de paginação.
+ **Efeito de zoom**: Tipo de efeito de zoom quando o mouse paira sobre a imagem.
+ **Bordas arredondadas**: Aplicar bordas arredondadas às imagens.
+ **Inclinação**: Aplicar um efeito de inclinação na imagem.
+ **Efeito de cor**: Tipo de efeito de cor quando o mouse paira sobre a imagem.
+ **Legenda**: Exibir parte da legenda da postagem.
+ **Link para postagem original**: Acessar as postagens originais clicando nas imagens.
+ **Móvel**: Exibir a galeria em dispositivos com resolução de tela inferior a 576px.

# Exibir a galeria no layout.
Vá para **_Design_ > _Layouts_**, encontre o layout onde deseja exibir a galeria e clique em **_Editar_** no final da linha.
<p align="center"><img src="images/layout_list.png" width="600" alt="Lista de layouts" title="Lista de layouts"></p>

Escolha a posição na qual a galeria será exibida. No menu suspenso, localize a galeria pelo nome, clique no botão **_Adicionar módulo_** e salve as alterações.
Neste exemplo, configuraremos a galeria para ser exibida na parte inferior do conteúdo.
<p align="center"><img src="images/layout_form.png" width="600" alt="Formulário de layout" title="Formulário de layout"></p>

# Permissões de acesso e modificação
Vá para **Sistema > Usuários > Grupos de usuários**, localize seu grupo pelo nome e clique em **_Editar_** no final da linha.

Nas listas **_Permissões de acesso_** e **_Permissões de modificação_**, localize a linha **_extension/module/instagram_gallery_multilang_** e certifique-se de que está marcada.
<p align="center"><img src="images/permissions.png" width="600" alt="Permissões" title="Permissões"></p>

# Desinstalar
<p align="center"><img src="images/caution.png" width="400" alt="caution" title="caution"></p>
Ao desinstalar o módulo, todas as configurações, galerias e mídias serão excluídas.

Vá para **_Extensões > Instalador_**, localize o módulo e clique em **_Desinstalar_** no final da linha.
<p align="center"><img src="images/uninstall.png" width="600" alt="Desinstalar" title="Desinstalar"></p>

# Solução de problemas
Acesse a [página de solução de problemas](https://github.com/ab-rodrigo/instagram-gallery-multilang-docs/blob/main/troubleshooting.md).

# Licença
GNU General Public License version 3 (GPLv3) - https://www.gnu.org/

# Como obter ajuda
Por favor, acesse a [página do módulo](https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=44767&filter_member=Rodrigoabr) e clique no botão "Obter suporte".

# Contato
Rodrigo Barbosa - ab.rodrigo@outlook.com

# Buy me a coffee
<p align="center"><a href="https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW" target="_blank"><img src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" alt="Botão de doação do PayPal" title="PayPal - A maneira mais segura e fácil de pagar online!"></a></p>

