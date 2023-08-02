<p align="center">
  <a href="https://github.com/pf666nb/pf666nb/blob/main/251657944137_.pic.jpg"><img src="https://github.com/pf666nb/pf666nb/blob/main/251657944137_.pic.jpg" alt="电锯人"></a>
</p>

<h1 align="center">Hi, I'm Yuks!</h1>
<h1 align="center">例外占多数者规则</h1>

<p align="center">
  <a href="https://github.com/pf666nb"><img src="https://github-readme-stats.vercel.app/api?username=pf666nb&hide_border=true&show_icons=true" alt="pf666nb's github stats"></a>
</p>
- uses: Platane/snk@v3
  with:
    # github user name to read the contribution graph from (**required**)
    # using action context var `github.repository_owner` or specified user
    github_user_name: ${{ github.repository_owner }}

    # list of files to generate.
    # one file per line. Each output can be customized with options as query string.
    #
    #  supported options:
    #  - palette:     A preset of color, one of [github, github-dark, github-light]
    #  - color_snake: Color of the snake
    #  - color_dots:  Coma separated list of dots color.
    #                 The first one is 0 contribution, then it goes from the low contribution to the highest.
    #                 Exactly 5 colors are expected.
    outputs: |
      dist/github-snake.svg
      dist/github-snake-dark.svg?palette=github-dark
      dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9

env:
# a github token is required to fetch the contribution calendar from github API
GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

