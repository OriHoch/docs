---
title: Gerenciando o acesso ao repositório para os codespaces da sua organização
shortTitle: Acesso ao repositório
intro: 'Você pode gerenciar os repositórios na sua organização que {% data variables.product.prodname_github_codespaces %} pode acessar.'
product: '{% data reusables.gated-features.codespaces %}'
permissions: 'To manage access and security for {% data variables.product.prodname_github_codespaces %} for an organization, you must be an organization owner.'
versions:
  fpt: '*'
  ghec: '*'
type: how_to
topics:
  - Codespaces
  - Security
  - Administrator
redirect_from:
  - /codespaces/managing-codespaces-for-your-organization/managing-access-and-security-for-your-organizations-codespaces
  - /github/developing-online-with-codespaces/managing-access-and-security-for-codespaces
  - /codespaces/working-with-your-codespace/managing-access-and-security-for-codespaces
---

{% warning %}

**Deprecation note**: The access and security setting described below is now deprecated and is documented here for reference only. Para habilitar o acesso expandido a outros repositórios, adicione as permissões solicitadas à definição do contêiner de desenvolvimento. Para obter mais informações, consulte "[Gerenciar o acesso a outros repositórios dentro de seu codespace](/codespaces/managing-your-codespaces/managing-repository-access-for-your-codespaces)".

{% endwarning %}

Por padrão, um codespace só pode acessar o repositório onde foi criado. Ao habilitar o acesso e a segurança de um repositório pertencente à sua organização, todos os codespaces que forem criados para esse repositório também terão permissões de leitura para todos os outros repositórios que a organização possui e o criador de codespace terá permissões para acessar. Se você deseja restringir os repositórios que um codespace pode acessar, você pode limitá-lo ao repositório em que o codespace foi criado ou a repositórios específicos. Você só deve habilitar o acesso e a segurança para repositórios nos quais confia.

To manage which users in your organization can use {% data variables.product.prodname_github_codespaces %}, see "[Enabling GitHub Codespaces for your organization](/codespaces/managing-codespaces-for-your-organization/enabling-github-codespaces-for-your-organization#enable-codespaces-for-users-in-your-organization)."

{% data reusables.profile.access_org %}
{% data reusables.profile.org_settings %}
{% data reusables.organizations.click-codespaces %}
1. Em "Acesso e segurança", selecione a configuração que você deseja para a sua organização. ![Botões de opção para gerenciar repositórios confiáveis](/assets/images/help/settings/codespaces-org-access-and-security-radio-buttons.png)
1. Se você escolheu "repositórios selecionados", selecione o menu suspenso e, em seguida, clique em um repositório para permitir que os codespaces do repositório acessem outros repositórios pertencentes à sua organização. Repita isso para todos os repositórios cujos códigos você deseja que acessem outros repositórios. ![Menu suspenso "Repositórios selecionados"](/assets/images/help/settings/codespaces-access-and-security-repository-drop-down.png)

## Leia mais

- "[Gerenciando acesso ao repositório para seus codespaces](/codespaces/managing-your-codespaces/managing-repository-access-for-your-codespaces)"
