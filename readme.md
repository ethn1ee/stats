# Stats

![Harlok's WakaTime stats](https://stats.taehoonlee.dev/api/wakatime?username=ethn1ee)

![Harlok's WakaTime stats](https://stats.taehoonlee.dev/api/wakatime?username=ethn1ee\&hide_progress=true)

*   Compact layout

![Harlok's WakaTime stats](https://stats.taehoonlee.dev/api/wakatime?username=ethn1ee\&layout=compact)

***

# All Demos

*   Default

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee)

*   Hiding specific stats

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&hide=contribs,issues)

*   Showing additional stats

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&show_icons=true\&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)

*   Showing icons

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&hide=issues\&show_icons=true)

*   Shows GitHub logo instead rank level

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&rank_icon=github)

*   Shows user rank percentile instead of rank level

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&rank_icon=percentile)

*   Customize Border Color

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&border_color=2e4058)

*   Include All Commits

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&include_all_commits=true)

*   Themes

Choose from any of the [default themes](#themes)

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&show_icons=true\&theme=radical)

*   Gradient

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api?username=ethn1ee\&bg_color=30,e96443,904e95\&title_color=fff\&text_color=fff)

*   Customizing stats card

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api/?username=ethn1ee\&show_icons=true\&title_color=fff\&icon_color=79ff97\&text_color=9f9f9f\&bg_color=151515)

*   Setting card locale

![Anurag's GitHub stats](https://stats.taehoonlee.dev/api/?username=ethn1ee\&locale=es)

*   Customizing repo card

![Customized Card](https://stats.taehoonlee.dev/api/pin?username=ethn1ee\&repo=github-readme-stats\&title_color=fff\&icon_color=f9f9f9\&text_color=9f9f9f\&bg_color=151515)

*   Gist card

![Gist Card](https://stats.taehoonlee.dev/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)

*   Customizing gist card

![Gist Card](https://stats.taehoonlee.dev/api/gist?id=bbfce31e0217a3689c8d961a356cb10d&theme=calm)

*   Top languages

![Top Langs](https://stats.taehoonlee.dev/api/top-langs/?username=ethn1ee)

*   WakaTime card

![Harlok's WakaTime stats](https://stats.taehoonlee.dev/api/wakatime?username=ethn1ee)

***

## Quick Tip (Align The Cards)

By default, GitHub does not lay out the cards side by side. To do that, you can use such approaches:

### Stats and top languages cards

```html
<a href="https://github.com/anuraghazra/github-readme-stats">
  <img height=200 align="center" src="https://stats.taehoonlee.dev/api?username=ethn1ee" />
</a>
<a href="https://github.com/anuraghazra/convoychat">
  <img height=200 align="center" src="https://stats.taehoonlee.dev/api/top-langs?username=ethn1ee&layout=compact&langs_count=8&card_width=320" />
</a>
```

<details>
<summary>:eyes: Show example</summary>

<a href="https://github.com/anuraghazra/github-readme-stats">
  <img height=200 align="center" src="https://stats.taehoonlee.dev/api?username=ethn1ee" />
</a>
<a href="https://github.com/anuraghazra/convoychat">
  <img height=200 align="center" src="https://stats.taehoonlee.dev/api/top-langs?username=ethn1ee&layout=compact&langs_count=8&card_width=320" />
</a>

</details>

### Pinning repositories

```html
<a href="https://github.com/anuraghazra/github-readme-stats">
  <img align="center" src="https://stats.taehoonlee.dev/api/pin/?username=ethn1ee&repo=github-readme-stats" />
</a>
<a href="https://github.com/anuraghazra/convoychat">
  <img align="center" src="https://stats.taehoonlee.dev/api/pin/?username=ethn1ee&repo=convoychat" />
</a>
```

<details>
<summary>:eyes: Show example</summary>

<a href="https://github.com/anuraghazra/github-readme-stats">
  <img align="center" src="https://stats.taehoonlee.dev/api/pin/?username=ethn1ee&repo=github-readme-stats" />
</a>
<a href="https://github.com/anuraghazra/convoychat">
  <img align="center" src="https://stats.taehoonlee.dev/api/pin/?username=ethn1ee&repo=convoychat" />
</a>

</details>

# Deploy on your own

## First step: get your Personal Access Token (PAT)

For deploying your own instance of GitHub Readme Stats, you will need to create a GitHub Personal Access Token (PAT). Below are the steps to create one and the scopes you need to select for both classic and fine-grained tokens.

Selecting the right scopes for your token is important in case you want to display private contributions on your cards.

### Classic token

* Go to [Account -> Settings -> Developer Settings -> Personal access tokens -> Tokens (classic)](https://github.com/settings/tokens).
* Click on `Generate new token -> Generate new token (classic)`.
* Scopes to select:
  * repo
  * read:user
* Click on `Generate token` and copy it.

### Fine-grained token

> [!WARNING]\
> This limits the scope to issues in your repositories and includes only public commits.

* Go to [Account -> Settings -> Developer Settings -> Personal access tokens -> Fine-grained tokens](https://github.com/settings/tokens).
* Click on `Generate new token -> Generate new token`.
* Select an expiration date
* Select `All repositories`
* Scopes to select in `Repository permission`:
  * Commit statuses: read-only
  * Contents: read-only
  * Issues: read-only
  * Metadata: read-only
  * Pull requests: read-only
* Click on `Generate token` and copy it.

## On Vercel

### :film\_projector: [Check Out Step By Step Video Tutorial By @codeSTACKr](https://youtu.be/n6d4KHSKqGk?t=107)

Since the GitHub API only allows 5k requests per hour, my `https://stats.taehoonlee.dev/api` could possibly hit the rate limiter. If you host it on your own Vercel server, then you do not have to worry about anything. Click on the deploy button to get started!

> [!NOTE]
> Since [#58](https://github.com/anuraghazra/github-readme-stats/pull/58), we should be able to handle more than 5k requests and have fewer issues with downtime :grin:.

> [!NOTE]
> If you are on the [Pro (i.e. paid)](https://vercel.com/pricing) Vercel plan, the [maxDuration](https://vercel.com/docs/concepts/projects/project-configuration#value-definition) value found in the [vercel.json](https://github.com/anuraghazra/github-readme-stats/blob/master/vercel.json) can be increased when your Vercel instance frequently times out during the card request. You are advised to keep this value lower than `30` seconds to prevent high memory usage.

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/anuraghazra/github-readme-stats)

<details>
 <summary><b>:hammer_and_wrench: Step-by-step guide on setting up your own Vercel instance</b></summary>

1.  Go to [vercel.com](https://vercel.com/).
2.  Click on `Log in`.
    ![](https://files.catbox.moe/pcxk33.png)
3.  Sign in with GitHub by pressing `Continue with GitHub`.
    ![](https://files.catbox.moe/b9oxey.png)
4.  Sign in to GitHub and allow access to all repositories if prompted.
5.  Fork this repo.
6.  Go back to your [Vercel dashboard](https://vercel.com/dashboard).
7.  To import a project, click the `Add New...` button and select the `Project` option.
    ![](https://files.catbox.moe/3n76fh.png)
8.  Click the `Continue with GitHub` button, search for the required Git Repository and import it by clicking the `Import` button. Alternatively, you can import a Third-Party Git Repository using the `Import Third-Party Git Repository ->` link at the bottom of the page.
    ![](https://files.catbox.moe/mg5p04.png)
9.  Create a Personal Access Token (PAT) as described in the [previous section](#first-step-get-your-personal-access-token-pat).
10. Add the PAT as an environment variable named `PAT_1` (as shown).
    ![](https://files.catbox.moe/0yclio.png)
11. Click deploy, and you're good to go. See your domains to use the API!

</details>

## On other platforms

> [!WARNING]
> This way of using GRS is not officially supported and was added to cater to some particular use cases where Vercel could not be used (e.g. [#2341](https://github.com/anuraghazra/github-readme-stats/discussions/2341)). The support for this method, therefore, is limited.

<details>
<summary><b>:hammer_and_wrench: Step-by-step guide for deploying on other platforms</b></summary>

1.  Fork or clone this repo as per your needs
2.  Move `express` from the devDependencies to the dependencies section of `package.json`
    <https://github.com/anuraghazra/github-readme-stats/blob/ba7c2f8b55eac8452e479c8bd38b044d204d0424/package.json#L54-L61>
3.  Run `npm i` if needed (initial setup)
4.  Run `node express.js` to start the server, or set the entry point to `express.js` in `package.json` if you're deploying on a managed service
    <https://github.com/anuraghazra/github-readme-stats/blob/ba7c2f8b55eac8452e479c8bd38b044d204d0424/package.json#L11>
5.  You're done 🎉
    </details>

## Available environment variables

GitHub Readme Stats provides several environment variables that can be used to customize the behavior of your self-hosted instance. These include:

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
      <th>Supported values</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>CACHE_SECONDS</code></td>
      <td>Sets the cache duration in seconds for the generated cards. This variable takes precedence over the default cache timings for the public instance. If this variable is not set, the default cache duration is 24 hours (86,400 seconds).</td>
      <td>Any positive integer or <code>0</code> to disable caching</td>
    </tr>
    <tr>
      <td><code>WHITELIST</code></td>
      <td>A comma-separated list of GitHub usernames that are allowed to access your instance. If this variable is not set, all usernames are allowed.</td>
      <td>Comma-separated GitHub usernames</td>
    </tr>
    <tr>
      <td><code>GIST_WHITELIST</code></td>
      <td>A comma-separated list of GitHub Gist IDs that are allowed to be accessed on your instance. If this variable is not set, all Gist IDs are allowed.</td>
      <td>Comma-separated GitHub Gist IDs</td>
    </tr>
    <tr>
      <td><code>EXCLUDE_REPO</code></td>
      <td>A comma-separated list of repositories that will be excluded from stats and top languages cards on your instance. This allows repository exclusion without exposing repository names in public URLs. This enhances privacy for self-hosted instances that include private repositories in stats cards.</td>
      <td>Comma-separated repository names</td>
    </tr>
    <tr>
      <td><code>FETCH_MULTI_PAGE_STARS</code></td>
      <td>Enables fetching all starred repositories for accurate star counts, especially for users with more than 100 repositories. This may increase response times and API points usage, so it is disabled on the public instance.</td>
      <td><code>true</code> or <code>false</code></td>
    </tr>
  </tbody>
</table>

See [the Vercel documentation](https://vercel.com/docs/concepts/projects/environment-variables) on adding these environment variables to your Vercel instance.

> [!WARNING]
> Please remember to redeploy your instance after making any changes to the environment variables so that the updates take effect. The changes will not be applied to the previous deployments.

## Keep your fork up to date

You can keep your fork, and thus your private Vercel instance up to date with the upstream using GitHub's [Sync Fork button](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork). You can also use the [pull](https://github.com/wei/pull) package created by [@wei](https://github.com/wei) to automate this process.

# :sparkling\_heart: Support the project

I open-source almost everything I can and try to reply to everyone needing help using these projects. Obviously,
this takes time. You can use this service for free.

However, if you are using this project and are happy with it or just want to encourage me to continue creating stuff, there are a few ways you can do it:

*   Giving proper credit when you use github-readme-stats on your readme, linking back to it. :D
*   Starring and sharing the project. :rocket:
*   [![paypal.me/anuraghazra](https://ionicabizau.github.io/badges/paypal.svg)](https://www.paypal.me/anuraghazra) - You can make a one-time donation via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:

Thanks! :heart:

***

[![https://vercel.com?utm\_source=github\_readme\_stats\_team\&utm\_campaign=oss](powered-by-vercel.svg)](https://vercel.com?utm_source=github_readme_stats_team\&utm_campaign=oss)

Contributions are welcome! <3

Made with :heart: and JavaScript.
