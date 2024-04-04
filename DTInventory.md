Apresentação do Projeto DTInventory: Sistema de Controle de Estoque

Problema: Todos os materiais de TI comprados pelos demais departamentos da empresa são guardados no DTI, até que seja solicitada a retirada para uso.Também recolhemos os kits de colaboradores desligados e guardamos até o momento de fazer o replace para outra pessoa. Tínhamos um pequeno espaço para guardar muitos materiais de diversos departamentos e pessoas diferentes: Cerca de 600 itens. O controle era feito a partir de uma planilha e acabávamos perdendo o controle devido ao grande volume e pessoas diferentes movimentando.

Solução: Como projeto de melhoria foi desenvolvimento um sistema de controle de estoque low code, feito no Power Apps da Microsoft, Sharepoint e Power Automate, todos ferramentas corporativas do office 365 (sem custo adicional financeiro para empresa, pois todos já tínhamos licença). A solução faz a leitura do código de barras das plaquetas (ativo fixo) e retorna várias informações na tela como: RC, NF, Líder do projeto (dono que comprou), SN, Data de entrada, quem recebeu e outros. Foi também criado uma tela para saída dos itens onde já traz todas as informações cadastradas e tem a opção e inserir assinatura eletrônica na tela touch-screen (dedo, caneta digital ou mouse), substituindo nosso formulário de papel de registro de entrega. Pode-se anexar arquivos (fotos e pdf) e informar o colaborador que está recebendo (todos os nomes de pessoas são integrados através do e-mail de forma automática). Ao realizar uma entrada/saída é disparado um fluxo de aprovals no power automate, um aprovalls chega no Teams do aprovador, a respota é enviada em um formulário para todos os envolvidos com resumo das informações. 1.2. Tela Inicial


Tela de ações:

![2 - Copia](https://github.com/aoliveira2021/Projetos/assets/85410083/814c4b3e-0d76-4925-b328-cecac9318dfe)
![1 - Copia](https://github.com/aoliveira2021/Projetos/assets/85410083/e6af79a3-614b-4a18-9b5f-24b380b49401)

Tela de cadastro:
![3](https://github.com/aoliveira2021/Projetos/assets/85410083/d6313fc9-129d-47dd-8a57-a92efb648191)
![8](https://github.com/aoliveira2021/Projetos/assets/85410083/ce19c561-3229-4556-861d-e1197ccbcaae)
![10](https://github.com/aoliveira2021/Projetos/assets/85410083/8bcfed08-5261-4364-bfe0-718f6ca53f03)



Tela de Consulta:
![5](https://github.com/aoliveira2021/Projetos/assets/85410083/1a30efc4-7b38-49c7-9342-89ea9b265e09)


Export diário de relatório dos equipamentos:
Foi realizado uma autmação no power Apps para todos os dias de segunda a sexta enviar pelo Outlook o relatório anexao (excel) dos equipamentos para todos os Líderes de projetos.

![11 - Copia](https://github.com/aoliveira2021/Projetos/assets/85410083/bb182f88-7be5-437b-b0cd-f6b9badfe2d3)
![12 - Copia](https://github.com/aoliveira2021/Projetos/assets/85410083/887d75a0-afc3-4aad-a290-b3978a7fcdab)


Configuração no Power Automate:

Solicitação de aprovação (Utilizando do Approvalls dentro do Teams):

Quando realizada uma entrada ou saída de equipamento, uma aprovação é enviada no Approvals do Teams da pessoa que está selecionada no campo “PL” que é referente ao líder de projeto:
![image](https://github.com/aoliveira2021/Projetos/assets/85410083/9624810c-ca94-4334-b7a5-e1d30159c0c6)
![image](https://github.com/aoliveira2021/Projetos/assets/85410083/d1bd06b5-ee7e-4efe-a717-a58dfd34e8b1)
![image](https://github.com/aoliveira2021/Projetos/assets/85410083/1647b926-c787-41c4-8968-a712639ced3d)
![image](https://github.com/aoliveira2021/Projetos/assets/85410083/939a11f3-70b5-46e7-8ffe-3507e8454c3f)
![image](https://github.com/aoliveira2021/Projetos/assets/85410083/2f0d862c-90a0-4bb8-b15d-0623b383f036)
![image](https://github.com/aoliveira2021/Projetos/assets/85410083/3cf8aed5-6fa0-4c3c-810c-edfee4652e34)


Depois de aprovado é enviado um e-mail copiando o PL, agentes de TI e solicitante. Notificando a movimentação


Organização do Estoque Físico:
Para que o sistema faça o controle foi necessário organizar o estoque físico. Realizado a compra de estantes metálicas com prateleiras e gavetas. Cada prateleira e gaveta foi etiquetada com seu devido código para poder ser cadastrado no sistema.

![DTInventory_page-0008 (1)](https://github.com/aoliveira2021/Projetos/assets/85410083/882080d9-80b8-4a25-a01a-83731b7f2e9a)
![DTInventory_page-0009](https://github.com/aoliveira2021/Projetos/assets/85410083/9ed096fa-7eff-4e5d-a3ac-20512191ca0c)
![DTInventory_page-0010](https://github.com/aoliveira2021/Projetos/assets/85410083/b91fd4aa-8095-436e-ab22-156c7f503503)



