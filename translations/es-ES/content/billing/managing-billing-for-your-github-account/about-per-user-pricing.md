---
title: Acerca del precio por usuario
intro: 'With per-user pricing, organizations {% ifversion ghec %}and enterprises {% endif %}pay based on team size to access advanced collaboration and management tools for teams, and optionally, security, compliance, and deployment controls.'
redirect_from:
  - /github/setting-up-and-managing-billing-and-payments-on-github/about-per-user-pricing
  - /articles/about-per-user-pricing
  - /github/setting-up-and-managing-billing-and-payments-on-github/managing-billing-for-your-github-account/about-per-user-pricing
versions:
  fpt: '*'
  ghec: '*'
type: overview
topics:
  - Downgrades
  - Enterprise
  - Licensing
  - Organizations
---

## Acerca del precio por usuario

New organizations on {% data variables.product.prodname_dotcom_the_website %} can build public and open-source projects with {% data variables.product.prodname_free_team %}, or upgrade to a paid product with per-user pricing. For more information, see "[{% data variables.product.company_short %}'s products](/get-started/learning-about-github/githubs-products)" and "[Upgrading your {% data variables.product.prodname_dotcom %} subscription](/billing/managing-billing-for-your-github-account/upgrading-your-github-subscription)."

{% ifversion ghec %}Per-user pricing applies to all organizations that belong to your enterprise on {% data variables.product.prodname_dotcom_the_website %}, and to organizations using  {% data variables.product.prodname_ghe_cloud %} that are not part of an enterprise. Each{% elsif fpt %}Per-user pricing means that each{% endif %} billing cycle, {% data variables.product.company_short %} charges for each member or outside collaborator within your organization{% ifversion ghec %} or enterprise{% endif %}. You also pay for each pending member or outside collaborator who has not yet accepted an invitation. {% data variables.product.company_short %} does not charge for members with the billing manager role{% ifversion ghec %}, or for enterprise owners who are not also a member of at least one organization in the enterprise{% endif %}. For more information, see {% ifversion ghec %}"[Roles in an enterprise](/admin/user-management/managing-users-in-your-enterprise/roles-in-an-enterprise)" or {% endif %}{% ifversion fpt or ghec %}"[Roles in an organization](/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization)."{% endif %}

{% data variables.product.company_short %} counts each {% ifversion ghec %}member or {% endif %}outside collaborator once for billing purposes, even if the person has {% ifversion ghec %}membership in multiple organizations in an enterprise or {% endif %}access to multiple repositories owned by your organization.

For more information about outside collaborators, see "[Adding outside collaborators to repositories in your organization](/organizations/managing-access-to-your-organizations-repositories/adding-outside-collaborators-to-repositories-in-your-organization)."

{% ifversion ghec %}

If you deploy {% data variables.product.prodname_ghe_server %}, your usage includes licenses for each user on your instance. For more information about additional services and billing for {% data variables.product.prodname_ghe_cloud %}, see "[About billing for your enterprise](/billing/managing-billing-for-your-github-account/about-billing-for-your-enterprise)."

{% elsif fpt %}

Las organizaciones que usan una suscripción paga antes del 11 de mayo de 2016 pueden elegir permanecer en su plan existente por repositorio o cambiar al precio por usuario. {% data variables.product.company_short %} will notify you twelve months before any mandated change to your subscription. Para obtener más información sobre cómo cambiar tu suscripción, consulta "[Actualizar tu {% data variables.product.prodname_dotcom %} suscripción](/billing/managing-billing-for-your-github-account/upgrading-your-github-subscription)".

{% endif %}

## Overview of per-user pricing

{% data reusables.billing.per-user-pricing-reference %}

## About changes to your subscription

{% ifversion fpt %}

You can change your {% data variables.product.prodname_dotcom %} subscription at any time.

### About changes for organizations on per-user plans

{% endif %}

You can add more users to your organization{% ifversion ghec %} or enterprise at any time{% endif %}. If you pay for more users than are currently active, you can also reduce the number of paid users.{% ifversion fpt %} For more information, see "[Upgrading your {% data variables.product.prodname_dotcom %} subscription](/billing/managing-billing-for-your-github-account/upgrading-your-github-subscription)" and "[Downgrading your {% data variables.product.prodname_dotcom %} subscription](/billing/managing-billing-for-your-github-account/downgrading-your-github-subscription)."

If you have questions about your subscription, contact {% data variables.contact.contact_support %}.

Para apoyar aún más las capacidades de colaboración de tu equipo, puedes mejorar a {% data variables.product.prodname_ghe_cloud %}, el cual incluye características como las ramas protegidas y los propietarios de código en los repositorios privados. {% data reusables.enterprise.link-to-ghec-trial %}

For more information about per-user pricing for {% data variables.product.prodname_ghe_cloud %}, see [the {% data variables.product.prodname_ghe_cloud %} documentation](/enterprise-cloud@latest/billing/managing-billing-for-your-github-account/about-per-user-pricing).

{% elsif ghec %}

If you use an enterprise account on {% data variables.product.prodname_dotcom_the_website %} and have questions about changes to your subscription, contact {% data variables.contact.contact_enterprise_sales %}.

If you use an individual organization on {% data variables.product.prodname_ghe_cloud %}, you can upgrade or downgrade your subscription. For more information, see "[Upgrading your {% data variables.product.prodname_dotcom %} subscription](/billing/managing-billing-for-your-github-account/upgrading-your-github-subscription)" or "[Downgrading your {% data variables.product.prodname_dotcom %} subscription](/billing/managing-billing-for-your-github-account/downgrading-your-github-subscription)." If you have questions about your subscription, contact {% data variables.contact.contact_support %}.

{% endif %}

{% ifversion fpt %}

### About changes for organizations on per-repository plans

Puedes actualizar o bajar de categoría entre planes pagos heredados en los parámetros de facturación de tu organización. When you upgrade to a plan with more private repositories, {% data variables.product.company_short %} immediately moves your account to your new plan and bills you for the difference in price, prorated for the number of days left in your billing cycle.

Cuando bajas de categoría a un plan pago heredado con menos repositorios privados, tu nuevo plan entrará en vigencia en tu próxima fecha de facturación. Si tienes más repositorios privados de los que permite tu nuevo plan, tus repositorios privados se bloquearán cuando tu nuevo plan entre en vigencia. Para reducir la cantidad de repositorios privados, puedes hacer que algunos de tus repositorios privados sean públicos o puedes clonar tus repositorios privados localmente y eliminar las copias en {% data variables.product.prodname_dotcom %}.

{% endif %}

## Leer más

{%- ifversion ghec %}
- "[Acerca de las cuentas de empresa](/admin/overview/about-enterprise-accounts)"
{%- endif %}
- "[Acerca de los repositorios](/repositories/creating-and-managing-repositories/about-repositories#about-repository-visibility)"
