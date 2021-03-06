---
title: 在个人资料中查看贡献
intro: 'Your {% data variables.product.product_name %} profile shows off {% if currentVersion == "free-pro-team@latest" or enterpriseServerVersions contains currentVersion %}your pinned repositories as well as{% endif %} a graph of your repository contributions over the past year.'
redirect_from:
  - /articles/viewing-contributions/
  - /articles/viewing-contributions-on-your-profile-page/
  - /articles/viewing-contributions-on-your-profile
versions:
  free-pro-team: '*'
  enterprise-server: '*'
  github-ae: '*'
---

{% if currentVersion == "free-pro-team@latest" or enterpriseServerVersions contains currentVersion %}Your contribution graph shows activity from public repositories. {% endif %}You can choose to show activity from {% if currentVersion == "free-pro-team@latest" or enterpriseServerVersions contains currentVersion %}both public and {% endif %}private repositories, with specific details of your activity in private repositories anonymized. 更多信息请参阅“[在个人资料中公开或隐藏私有贡献](/articles/publicizing-or-hiding-your-private-contributions-on-your-profile)”。

{% note %}

**Note:** Commits will only appear on your contributions graph if the email address you used to author the commits is connected to your account on {% data variables.product.product_name %}. 更多信息请参阅“[为什么我的贡献没有在我的个人资料中显示？](/articles/why-are-my-contributions-not-showing-up-on-my-profile#your-local-git-commit-email-isnt-connected-to-your-account)”

{% endnote %}

### 计为贡献的内容

在您的个人资料页面上，某些操作计为贡献：

- 提交到仓库的默认分支或 `gh-pages` 分支
- 打开议题
- 提议拉取请求
- Submitting a pull request review{% if enterpriseServerVersions contains currentVersion or currentVersion == "github-ae@latest" %}
- 合作创作仓库默认分支或 `gh-pages` 分支中的提交{% endif %}

{% data reusables.pull_requests.pull_request_merges_and_contributions %}

### 受欢迎的仓库

此部分显示具有最多查看者的仓库。 {% if currentVersion == "free-pro-team@latest" or enterpriseServerVersions contains currentVersion %}Once you [pin repositories to your profile](/articles/pinning-repositories-to-your-profile), this section will change to "Pinned repositories."{% endif %}

![受欢迎的仓库](/assets/images/help/profile/profile_popular_repositories.png)

{% if currentVersion == "free-pro-team@latest" or enterpriseServerVersions contains currentVersion %}

### 固定的仓库

此部分显示最多六个公共仓库，并可包括您的仓库以及您对其做出贡献的仓库。 为便于查看关于您选择提供的仓库的重要详细信息，此部分中的每个仓库均包括所进行工作的摘要、仓库已收到的[星号](/articles/saving-repositories-with-stars/)数量以及仓库中使用的主要编程语言。 更多信息请参阅“[将仓库固定到个人资料](/articles/pinning-repositories-to-your-profile)”。

![固定的仓库](/assets/images/help/profile/profile_pinned_repositories.png)

{% endif %}

### 贡献日历

您的贡献日历会显示贡献活动。

#### 查看特定时间的贡献

- 单击某个日期的方块可显示该 24 小时期间内所做的贡献。
- 按 *Shift* 并单击任意日期的方块可显示该时间范围内所做的贡献。

{% note %}

**注：**您可以在贡献日历中选择最多一个月的范围。 如果您选择了更大的时间范围，我们将仅显示一个月的贡献。

{% endnote %}

![您的贡献图](/assets/images/help/profile/contributions_graph.png)

#### 如何计算贡献事件时间

对于提交和拉取请求，时间戳的计算方式不同：
- **提交**使用提交时间戳中的时区信息。 更多信息请参阅“[对时间表上的提交进行故障排除](/articles/troubleshooting-commits-on-your-timeline)”。
- 在 {% data variables.product.product_name %} 上打开的**拉取请求**和**议题**使用浏览器的时区。 通过 API 打开的内容使用 [API 调用中指定的](https://developer.github.com/changes/2014-03-04-timezone-handling-changes)时间戳或时区。

### 活动概览

{% data reusables.profile.activity-overview-summary %} 更多信息请参阅“[在个人资料中显示活动概览](/articles/showing-an-overview-of-your-activity-on-your-profile)”。

![个人资料中的活动概览部分](/assets/images/help/profile/activity-overview-section.png)

活动概览中提供的组织根据您在组织中的活跃程度确定优先级。 如果您在个人资料简历中@提及某个组织，并且您是组织成员，则该组织首先在活动概览中确定优先级。 更多信息请参阅“[提及人员和团队](/articles/basic-writing-and-formatting-syntax/#mentioning-people-and-teams)”或“[将个人简历添加到个人资料](/articles/adding-a-bio-to-your-profile/)”。

### 贡献活动

贡献活动部分包括工作的详细时间表，包括您进行或合作的提交、您提议的拉取请求以及您打开的议题。 您可通过单击贡献活动底部的 **Show more activity（显示更多活动）**或通过在查看页面右侧时单击您感兴趣的年份来查看一段时间内您的贡献。 重要时刻（如您加入组织、提议第一个拉取请求或打开一个备受瞩目议题的日期）将在贡献活动中突出显示。 如果您在时间表中无法看到某些事件，请检查以确保您仍具有事件发生位置组织或仓库的访问权限。

![贡献活动时间过滤器](/assets/images/help/profile/contributions_activity_time_filter.png)

{% if currentVersion != "github-ae@latest" %}
### 在 {% data variables.product.prodname_dotcom_the_website %} 上查看 {% data variables.product.product_location_enterprise %}的贡献
If your site administrator has enabled

{% data variables.product.prodname_unified_contributions %}, you can send {% data variables.product.prodname_enterprise %} contribution counts to your {% data variables.product.prodname_dotcom_the_website %} profile. 更多信息请参阅“[将 {% data variables.product.prodname_ghe_server %} 贡献发送到 {% data variables.product.prodname_dotcom_the_website %}](/articles/sending-your-github-enterprise-server-contributions-to-your-github-com-profile)”。
{% endif %}

### 延伸阅读

- "[在个人资料页面中查看贡献](/articles/viewing-contributions-on-your-profile-page)"
- “[为什么我的贡献没有在我的个人资料中显示？](/articles/why-are-my-contributions-not-showing-up-on-my-profile)”
- "[在个人资料中公开或隐藏私有贡献](/articles/publicizing-or-hiding-your-private-contributions-on-your-profile)"
- “[在个人资料中显示活动概览](/articles/showing-an-overview-of-your-activity-on-your-profile)”
