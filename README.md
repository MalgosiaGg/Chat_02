# Rasa Chatbot Widget 2.0

![ScreenShot](public/banner.png)
[![forthebadge](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNzguNjk5OTk5OTk5OTk5OTMiIGhlaWdodD0iMzUiIHZpZXdCb3g9IjAgMCAyNzguNjk5OTk5OTk5OTk5OTMgMzUiPjxyZWN0IGNsYXNzPSJzdmdfX3JlY3QiIHg9IjAiIHk9IjAiIHdpZHRoPSIyMDkuNDIiIGhlaWdodD0iMzUiIGZpbGw9IiM0QTI3OEMiLz48cmVjdCBjbGFzcz0ic3ZnX19yZWN0IiB4PSIyMDcuNDIiIHk9IjAiIHdpZHRoPSI3MS4yNzk5OTk5OTk5OTk5NyIgaGVpZ2h0PSIzNSIgZmlsbD0iI0I0QTVDOSIvPjxwYXRoIGNsYXNzPSJzdmdfX3RleHQiIGQ9Ik0xNS42OSAyMkwxNC4yMiAyMkwxNC4yMiAxMy40N0wxNi4xNCAxMy40N0wxOC42MCAyMC4wMUwyMS4wNiAxMy40N0wyMi45NyAxMy40N0wyMi45NyAyMkwyMS40OSAyMkwyMS40OSAxOS4xOUwyMS42NCAxNS40M0wxOS4xMiAyMkwxOC4wNiAyMkwxNS41NSAxNS40M0wxNS42OSAxOS4xOUwxNS42OSAyMlpNMjguNDkgMjJMMjYuOTUgMjJMMzAuMTcgMTMuNDdMMzEuNTAgMTMuNDdMMzQuNzMgMjJMMzMuMTggMjJMMzIuNDkgMjAuMDFMMjkuMTggMjAuMDFMMjguNDkgMjJaTTMwLjgzIDE1LjI4TDI5LjYwIDE4LjgyTDMyLjA3IDE4LjgyTDMwLjgzIDE1LjI4Wk00MS4xNCAyMkwzOC42OSAyMkwzOC42OSAxMy40N0w0MS4yMSAxMy40N1E0Mi4zNCAxMy40NyA0My4yMSAxMy45N1E0NC4wOSAxNC40OCA0NC41NyAxNS40MFE0NS4wNSAxNi4zMyA0NS4wNSAxNy41Mkw0NS4wNSAxNy41Mkw0NS4wNSAxNy45NVE0NS4wNSAxOS4xNiA0NC41NyAyMC4wOFE0NC4wOCAyMS4wMCA0My4xOSAyMS41MFE0Mi4zMCAyMiA0MS4xNCAyMkw0MS4xNCAyMlpNNDAuMTcgMTQuNjZMNDAuMTcgMjAuODJMNDEuMTQgMjAuODJRNDIuMzAgMjAuODIgNDIuOTMgMjAuMDlRNDMuNTUgMTkuMzYgNDMuNTYgMTcuOTlMNDMuNTYgMTcuOTlMNDMuNTYgMTcuNTJRNDMuNTYgMTYuMTMgNDIuOTYgMTUuNDBRNDIuMzUgMTQuNjYgNDEuMjEgMTQuNjZMNDEuMjEgMTQuNjZMNDAuMTcgMTQuNjZaTTU1LjA5IDIyTDQ5LjUxIDIyTDQ5LjUxIDEzLjQ3TDU1LjA1IDEzLjQ3TDU1LjA1IDE0LjY2TDUxLjAwIDE0LjY2TDUxLjAwIDE3LjAyTDU0LjUwIDE3LjAyTDU0LjUwIDE4LjE5TDUxLjAwIDE4LjE5TDUxLjAwIDIwLjgyTDU1LjA5IDIwLjgyTDU1LjA5IDIyWk02Ni43NSAyMkw2NS4yNiAyMkw2NS4yNiAxMy40N0w3MC42OCAxMy40N0w3MC42OCAxNC42Nkw2Ni43NSAxNC42Nkw2Ni43NSAxNy4yMEw3MC4xOCAxNy4yMEw3MC4xOCAxOC4zOEw2Ni43NSAxOC4zOEw2Ni43NSAyMlpNNzQuNTcgMTguMDBMNzQuNTcgMTguMDBMNzQuNTcgMTcuNTJRNzQuNTcgMTYuMjggNzUuMDIgMTUuMzJRNzUuNDYgMTQuMzcgNzYuMjcgMTMuODZRNzcuMDcgMTMuMzUgNzguMTEgMTMuMzVRNzkuMTYgMTMuMzUgNzkuOTYgMTMuODVRODAuNzcgMTQuMzUgODEuMjEgMTUuMjlRODEuNjUgMTYuMjMgODEuNjUgMTcuNDhMODEuNjUgMTcuNDhMODEuNjUgMTcuOTZRODEuNjUgMTkuMjEgODEuMjIgMjAuMTZRODAuNzkgMjEuMTAgNzkuOTggMjEuNjFRNzkuMTcgMjIuMTIgNzguMTMgMjIuMTJMNzguMTMgMjIuMTJRNzcuMDkgMjIuMTIgNzYuMjggMjEuNjFRNzUuNDcgMjEuMTAgNzUuMDIgMjAuMTdRNzQuNTggMTkuMjMgNzQuNTcgMTguMDBaTTc2LjA2IDE3LjQ2TDc2LjA2IDE3Ljk2UTc2LjA2IDE5LjM2IDc2LjYwIDIwLjEzUTc3LjE1IDIwLjkwIDc4LjEzIDIwLjkwTDc4LjEzIDIwLjkwUTc5LjExIDIwLjkwIDc5LjY0IDIwLjE1UTgwLjE3IDE5LjQwIDgwLjE3IDE3Ljk2TDgwLjE3IDE3Ljk2TDgwLjE3IDE3LjUxUTgwLjE3IDE2LjA5IDc5LjYzIDE1LjM0UTc5LjEwIDE0LjU4IDc4LjExIDE0LjU4TDc4LjExIDE0LjU4UTc3LjE1IDE0LjU4IDc2LjYxIDE1LjMzUTc2LjA3IDE2LjA5IDc2LjA2IDE3LjQ2TDc2LjA2IDE3LjQ2Wk04Ny42MCAyMkw4Ni4xMiAyMkw4Ni4xMiAxMy40N0w4OS4xMiAxMy40N1E5MC41OSAxMy40NyA5MS40MCAxNC4xM1E5Mi4yMCAxNC43OSA5Mi4yMCAxNi4wNUw5Mi4yMCAxNi4wNVE5Mi4yMCAxNi45MCA5MS43OSAxNy40OFE5MS4zNyAxOC4wNiA5MC42NCAxOC4zN0w5MC42NCAxOC4zN0w5Mi41NSAyMS45Mkw5Mi41NSAyMkw5MC45NiAyMkw4OS4yNSAxOC43MUw4Ny42MCAxOC43MUw4Ny42MCAyMlpNODcuNjAgMTQuNjZMODcuNjAgMTcuNTJMODkuMTIgMTcuNTJRODkuODcgMTcuNTIgOTAuMzAgMTcuMTVROTAuNzIgMTYuNzcgOTAuNzIgMTYuMTFMOTAuNzIgMTYuMTFROTAuNzIgMTUuNDMgOTAuMzMgMTUuMDVRODkuOTQgMTQuNjggODkuMTYgMTQuNjZMODkuMTYgMTQuNjZMODcuNjAgMTQuNjZaTTEwNS42OCAyMkwxMDIuNTcgMjJMMTAyLjU3IDEzLjQ3TDEwNS40OSAxMy40N1ExMDYuOTQgMTMuNDcgMTA3LjcwIDE0LjA1UTEwOC40NSAxNC42MyAxMDguNDUgMTUuNzhMMTA4LjQ1IDE1Ljc4UTEwOC40NSAxNi4zNiAxMDguMTQgMTYuODNRMTA3LjgyIDE3LjMwIDEwNy4yMSAxNy41NkwxMDcuMjEgMTcuNTZRMTA3LjkwIDE3Ljc1IDEwOC4yOCAxOC4yNlExMDguNjYgMTguNzggMTA4LjY2IDE5LjUxTDEwOC42NiAxOS41MVExMDguNjYgMjAuNzEgMTA3Ljg5IDIxLjM2UTEwNy4xMiAyMiAxMDUuNjggMjJMMTA1LjY4IDIyWk0xMDQuMDUgMTguMTVMMTA0LjA1IDIwLjgyTDEwNS43MCAyMC44MlExMDYuNDAgMjAuODIgMTA2Ljc5IDIwLjQ3UTEwNy4xOCAyMC4xMyAxMDcuMTggMTkuNTFMMTA3LjE4IDE5LjUxUTEwNy4xOCAxOC4xOCAxMDUuODIgMTguMTVMMTA1LjgyIDE4LjE1TDEwNC4wNSAxOC4xNVpNMTA0LjA1IDE0LjY2TDEwNC4wNSAxNy4wNkwxMDUuNTEgMTcuMDZRMTA2LjIwIDE3LjA2IDEwNi41OSAxNi43NVExMDYuOTggMTYuNDMgMTA2Ljk4IDE1Ljg2TDEwNi45OCAxNS44NlExMDYuOTggMTUuMjMgMTA2LjYyIDE0Ljk1UTEwNi4yNiAxNC42NiAxMDUuNDkgMTQuNjZMMTA1LjQ5IDE0LjY2TDEwNC4wNSAxNC42NlpNMTEyLjg2IDE4LjAwTDExMi44NiAxOC4wMEwxMTIuODYgMTcuNTJRMTEyLjg2IDE2LjI4IDExMy4zMCAxNS4zMlExMTMuNzQgMTQuMzcgMTE0LjU1IDEzLjg2UTExNS4zNiAxMy4zNSAxMTYuNDAgMTMuMzVRMTE3LjQ0IDEzLjM1IDExOC4yNSAxMy44NVExMTkuMDUgMTQuMzUgMTE5LjQ5IDE1LjI5UTExOS45MyAxNi4yMyAxMTkuOTQgMTcuNDhMMTE5Ljk0IDE3LjQ4TDExOS45NCAxNy45NlExMTkuOTQgMTkuMjEgMTE5LjUwIDIwLjE2UTExOS4wNyAyMS4xMCAxMTguMjcgMjEuNjFRMTE3LjQ2IDIyLjEyIDExNi40MSAyMi4xMkwxMTYuNDEgMjIuMTJRMTE1LjM3IDIyLjEyIDExNC41NiAyMS42MVExMTMuNzUgMjEuMTAgMTEzLjMxIDIwLjE3UTExMi44NyAxOS4yMyAxMTIuODYgMTguMDBaTTExNC4zNCAxNy40NkwxMTQuMzQgMTcuOTZRMTE0LjM0IDE5LjM2IDExNC44OSAyMC4xM1ExMTUuNDQgMjAuOTAgMTE2LjQxIDIwLjkwTDExNi40MSAyMC45MFExMTcuMzkgMjAuOTAgMTE3LjkzIDIwLjE1UTExOC40NiAxOS40MCAxMTguNDYgMTcuOTZMMTE4LjQ2IDE3Ljk2TDExOC40NiAxNy41MVExMTguNDYgMTYuMDkgMTE3LjkyIDE1LjM0UTExNy4zOCAxNC41OCAxMTYuNDAgMTQuNThMMTE2LjQwIDE0LjU4UTExNS40NCAxNC41OCAxMTQuOTAgMTUuMzNRMTE0LjM1IDE2LjA5IDExNC4zNCAxNy40NkwxMTQuMzQgMTcuNDZaTTEyNi4wOCAxNC42NkwxMjMuNDUgMTQuNjZMMTIzLjQ1IDEzLjQ3TDEzMC4yMiAxMy40N0wxMzAuMjIgMTQuNjZMMTI3LjU2IDE0LjY2TDEyNy41NiAyMkwxMjYuMDggMjJMMTI2LjA4IDE0LjY2Wk0xMzMuNTQgMTkuNDJMMTMzLjU0IDE5LjQyTDEzNS4wMiAxOS40MlExMzUuMDIgMjAuMTUgMTM1LjUwIDIwLjU1UTEzNS45OCAyMC45NSAxMzYuODggMjAuOTVMMTM2Ljg4IDIwLjk1UTEzNy42NSAyMC45NSAxMzguMDQgMjAuNjNRMTM4LjQzIDIwLjMyIDEzOC40MyAxOS44MEwxMzguNDMgMTkuODBRMTM4LjQzIDE5LjI0IDEzOC4wMyAxOC45NFExMzcuNjQgMTguNjMgMTM2LjYxIDE4LjMyUTEzNS41OCAxOC4wMSAxMzQuOTcgMTcuNjNMMTM0Ljk3IDE3LjYzUTEzMy44MCAxNi45MCAxMzMuODAgMTUuNzJMMTMzLjgwIDE1LjcyUTEzMy44MCAxNC42OSAxMzQuNjQgMTQuMDJRMTM1LjQ4IDEzLjM1IDEzNi44MiAxMy4zNUwxMzYuODIgMTMuMzVRMTM3LjcyIDEzLjM1IDEzOC40MSAxMy42OFExMzkuMTEgMTQuMDEgMTM5LjUxIDE0LjYxUTEzOS45MSAxNS4yMiAxMzkuOTEgMTUuOTZMMTM5LjkxIDE1Ljk2TDEzOC40MyAxNS45NlExMzguNDMgMTUuMjkgMTM4LjAxIDE0LjkxUTEzNy41OSAxNC41NCAxMzYuODEgMTQuNTRMMTM2LjgxIDE0LjU0UTEzNi4wOSAxNC41NCAxMzUuNjggMTQuODVRMTM1LjI4IDE1LjE2IDEzNS4yOCAxNS43MUwxMzUuMjggMTUuNzFRMTM1LjI4IDE2LjE4IDEzNS43MiAxNi41MFExMzYuMTUgMTYuODEgMTM3LjE1IDE3LjEwUTEzOC4xNCAxNy40MCAxMzguNzUgMTcuNzhRMTM5LjM1IDE4LjE2IDEzOS42MyAxOC42NVExMzkuOTEgMTkuMTMgMTM5LjkxIDE5Ljc5TDEzOS45MSAxOS43OVExMzkuOTEgMjAuODYgMTM5LjEwIDIxLjQ5UTEzOC4yOCAyMi4xMiAxMzYuODggMjIuMTJMMTM2Ljg4IDIyLjEyUTEzNS45NSAyMi4xMiAxMzUuMTggMjEuNzdRMTM0LjQwIDIxLjQzIDEzMy45NyAyMC44M1ExMzMuNTQgMjAuMjIgMTMzLjU0IDE5LjQyWk0xNTAuMDQgMTkuMTZMMTUwLjA0IDE5LjE2TDE1MC4wNCAxMy40N0wxNTEuNTIgMTMuNDdMMTUxLjUyIDE5LjE4UTE1MS41MiAyMC4wMyAxNTEuOTUgMjAuNDhRMTUyLjM5IDIwLjkzIDE1My4yMyAyMC45M0wxNTMuMjMgMjAuOTNRMTU0Ljk0IDIwLjkzIDE1NC45NCAxOS4xM0wxNTQuOTQgMTkuMTNMMTU0Ljk0IDEzLjQ3TDE1Ni40MiAxMy40N0wxNTYuNDIgMTkuMTdRMTU2LjQyIDIwLjUzIDE1NS41NSAyMS4zMlExNTQuNjggMjIuMTIgMTUzLjIzIDIyLjEyTDE1My4yMyAyMi4xMlExNTEuNzcgMjIuMTIgMTUwLjkwIDIxLjMzUTE1MC4wNCAyMC41NSAxNTAuMDQgMTkuMTZaTTE2MC41NiAxOS40MkwxNjAuNTYgMTkuNDJMMTYyLjA0IDE5LjQyUTE2Mi4wNCAyMC4xNSAxNjIuNTIgMjAuNTVRMTYzLjAwIDIwLjk1IDE2My44OSAyMC45NUwxNjMuODkgMjAuOTVRMTY0LjY3IDIwLjk1IDE2NS4wNiAyMC42M1ExNjUuNDUgMjAuMzIgMTY1LjQ1IDE5LjgwTDE2NS40NSAxOS44MFExNjUuNDUgMTkuMjQgMTY1LjA1IDE4Ljk0UTE2NC42NiAxOC42MyAxNjMuNjMgMTguMzJRMTYyLjU5IDE4LjAxIDE2MS45OCAxNy42M0wxNjEuOTggMTcuNjNRMTYwLjgyIDE2LjkwIDE2MC44MiAxNS43MkwxNjAuODIgMTUuNzJRMTYwLjgyIDE0LjY5IDE2MS42NiAxNC4wMlExNjIuNTAgMTMuMzUgMTYzLjg0IDEzLjM1TDE2My44NCAxMy4zNVExNjQuNzMgMTMuMzUgMTY1LjQzIDEzLjY4UTE2Ni4xMyAxNC4wMSAxNjYuNTMgMTQuNjFRMTY2LjkyIDE1LjIyIDE2Ni45MiAxNS45NkwxNjYuOTIgMTUuOTZMMTY1LjQ1IDE1Ljk2UTE2NS40NSAxNS4yOSAxNjUuMDMgMTQuOTFRMTY0LjYxIDE0LjU0IDE2My44MyAxNC41NEwxNjMuODMgMTQuNTRRMTYzLjEwIDE0LjU0IDE2Mi43MCAxNC44NVExNjIuMzAgMTUuMTYgMTYyLjMwIDE1LjcxTDE2Mi4zMCAxNS43MVExNjIuMzAgMTYuMTggMTYyLjczIDE2LjUwUTE2My4xNyAxNi44MSAxNjQuMTYgMTcuMTBRMTY1LjE2IDE3LjQwIDE2NS43NiAxNy43OFExNjYuMzcgMTguMTYgMTY2LjY1IDE4LjY1UTE2Ni45MyAxOS4xMyAxNjYuOTMgMTkuNzlMMTY2LjkzIDE5Ljc5UTE2Ni45MyAyMC44NiAxNjYuMTEgMjEuNDlRMTY1LjMwIDIyLjEyIDE2My44OSAyMi4xMkwxNjMuODkgMjIuMTJRMTYyLjk3IDIyLjEyIDE2Mi4xOSAyMS43N1ExNjEuNDIgMjEuNDMgMTYwLjk5IDIwLjgzUTE2MC41NiAyMC4yMiAxNjAuNTYgMTkuNDJaTTE3Mi43OCAyMkwxNzEuMzEgMjJMMTcxLjMxIDEzLjQ3TDE3Mi43OCAxMy40N0wxNzIuNzggMjJaTTE3OS4wOCAyMkwxNzcuNTkgMjJMMTc3LjU5IDEzLjQ3TDE3OS4wOCAxMy40N0wxODIuODkgMTkuNTRMMTgyLjg5IDEzLjQ3TDE4NC4zNiAxMy40N0wxODQuMzYgMjJMMTgyLjg4IDIyTDE3OS4wOCAxNS45NUwxNzkuMDggMjJaTTE4OC44NiAxOC4xM0wxODguODYgMTguMTNMMTg4Ljg2IDE3LjQ2UTE4OC44NiAxNS41MyAxODkuNzggMTQuNDRRMTkwLjcxIDEzLjM1IDE5Mi4zNyAxMy4zNUwxOTIuMzcgMTMuMzVRMTkzLjc5IDEzLjM1IDE5NC42MyAxNC4wNVExOTUuNDcgMTQuNzYgMTk1LjY0IDE2LjA4TDE5NS42NCAxNi4wOEwxOTQuMTggMTYuMDhRMTkzLjk0IDE0LjU0IDE5Mi4zOSAxNC41NEwxOTIuMzkgMTQuNTRRMTkxLjQwIDE0LjU0IDE5MC44OCAxNS4yNlExOTAuMzYgMTUuOTggMTkwLjM0IDE3LjM3TDE5MC4zNCAxNy4zN0wxOTAuMzQgMTguMDJRMTkwLjM0IDE5LjQwIDE5MC45MyAyMC4xN1ExOTEuNTEgMjAuOTMgMTkyLjU1IDIwLjkzTDE5Mi41NSAyMC45M1ExOTMuNjggMjAuOTMgMTk0LjE2IDIwLjQyTDE5NC4xNiAyMC40MkwxOTQuMTYgMTguNzVMMTkyLjQxIDE4Ljc1TDE5Mi40MSAxNy42MkwxOTUuNjQgMTcuNjJMMTk1LjY0IDIwLjg5UTE5NS4xOCAyMS41MCAxOTQuMzYgMjEuODFRMTkzLjU0IDIyLjEyIDE5Mi40OSAyMi4xMkwxOTIuNDkgMjIuMTJRMTkxLjQyIDIyLjEyIDE5MC42MCAyMS42M1ExODkuNzcgMjEuMTQgMTg5LjMyIDIwLjI0UTE4OC44NyAxOS4zMyAxODguODYgMTguMTNaIiBmaWxsPSIjRkZGRkZGIi8+PHBhdGggY2xhc3M9InN2Z19fdGV4dCIgZD0iTTIyMy45OSAyMkwyMjEuNjEgMjJMMjIxLjYxIDEzLjYwTDIyNS40NSAxMy42MFEyMjYuNTkgMTMuNjAgMjI3LjQzIDEzLjk4UTIyOC4yNyAxNC4zNSAyMjguNzMgMTUuMDZRMjI5LjE4IDE1Ljc2IDIyOS4xOCAxNi43MUwyMjkuMTggMTYuNzFRMjI5LjE4IDE3LjYyIDIyOC43NiAxOC4zMFEyMjguMzMgMTguOTggMjI3LjU0IDE5LjM2TDIyNy41NCAxOS4zNkwyMjkuMzUgMjJMMjI2LjgxIDIyTDIyNS4yOCAxOS43N0wyMjMuOTkgMTkuNzdMMjIzLjk5IDIyWk0yMjMuOTkgMTUuNDdMMjIzLjk5IDE3LjkzTDIyNS4zMSAxNy45M1EyMjYuMDQgMTcuOTMgMjI2LjQxIDE3LjYxUTIyNi43OCAxNy4yOSAyMjYuNzggMTYuNzFMMjI2Ljc4IDE2LjcxUTIyNi43OCAxNi4xMiAyMjYuNDEgMTUuNzlRMjI2LjA0IDE1LjQ3IDIyNS4zMSAxNS40N0wyMjUuMzEgMTUuNDdMMjIzLjk5IDE1LjQ3Wk0yMzUuMzkgMjJMMjMyLjk2IDIyTDIzNi42NyAxMy42MEwyMzkuMDIgMTMuNjBMMjQyLjczIDIyTDI0MC4yNiAyMkwyMzkuNjAgMjAuMzdMMjM2LjA1IDIwLjM3TDIzNS4zOSAyMlpNMjM3LjgzIDE1LjkzTDIzNi43NCAxOC42MUwyMzguOTAgMTguNjFMMjM3LjgzIDE1LjkzWk0yNDYuMzAgMjEuMjRMMjQ2LjMwIDIxLjI0TDI0Ny4wOCAxOS40OVEyNDcuNjQgMTkuODYgMjQ4LjM5IDIwLjA5UTI0OS4xMyAyMC4zMiAyNDkuODUgMjAuMzJMMjQ5Ljg1IDIwLjMyUTI1MS4yMiAyMC4zMiAyNTEuMjIgMTkuNjRMMjUxLjIyIDE5LjY0UTI1MS4yMiAxOS4yOCAyNTAuODMgMTkuMTFRMjUwLjQ0IDE4LjkzIDI0OS41NyAxOC43NEwyNDkuNTcgMTguNzRRMjQ4LjYzIDE4LjUzIDI0Ny45OSAxOC4zMFEyNDcuMzUgMTguMDYgMjQ2LjkwIDE3LjU1UTI0Ni40NSAxNy4wMyAyNDYuNDUgMTYuMTZMMjQ2LjQ1IDE2LjE2UTI0Ni40NSAxNS4zOSAyNDYuODYgMTQuNzdRMjQ3LjI4IDE0LjE1IDI0OC4xMiAxMy43OVEyNDguOTUgMTMuNDMgMjUwLjE2IDEzLjQzTDI1MC4xNiAxMy40M1EyNTAuOTkgMTMuNDMgMjUxLjc5IDEzLjYyUTI1Mi42MCAxMy44MCAyNTMuMjEgMTQuMTdMMjUzLjIxIDE0LjE3TDI1Mi40OCAxNS45M1EyNTEuMjggMTUuMjggMjUwLjE1IDE1LjI4TDI1MC4xNSAxNS4yOFEyNDkuNDQgMTUuMjggMjQ5LjEyIDE1LjQ5UTI0OC44MCAxNS43MCAyNDguODAgMTYuMDRMMjQ4LjgwIDE2LjA0UTI0OC44MCAxNi4zNyAyNDkuMTggMTYuNTRRMjQ5LjU2IDE2LjcxIDI1MC40MSAxNi44OUwyNTAuNDEgMTYuODlRMjUxLjM3IDE3LjEwIDI1Mi4wMCAxNy4zM1EyNTIuNjMgMTcuNTYgMjUzLjEwIDE4LjA3UTI1My41NiAxOC41OCAyNTMuNTYgMTkuNDZMMjUzLjU2IDE5LjQ2UTI1My41NiAyMC4yMSAyNTMuMTQgMjAuODNRMjUyLjcyIDIxLjQ0IDI1MS44OCAyMS44MFEyNTEuMDQgMjIuMTcgMjQ5Ljg0IDIyLjE3TDI0OS44NCAyMi4xN1EyNDguODIgMjIuMTcgMjQ3Ljg2IDIxLjkyUTI0Ni45MCAyMS42NyAyNDYuMzAgMjEuMjRaTTI1OS41NSAyMkwyNTcuMTMgMjJMMjYwLjg0IDEzLjYwTDI2My4xOCAxMy42MEwyNjYuODkgMjJMMjY0LjQzIDIyTDI2My43NyAyMC4zN0wyNjAuMjIgMjAuMzdMMjU5LjU1IDIyWk0yNjEuOTkgMTUuOTNMMjYwLjkxIDE4LjYxTDI2My4wNyAxOC42MUwyNjEuOTkgMTUuOTNaIiBmaWxsPSIjNEEyNzhDIiB4PSIyMjAuNDIiLz48L3N2Zz4=)](https://forthebadge.com)
[![forthebadge](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxOTYuOTMiIGhlaWdodD0iMzUiIHZpZXdCb3g9IjAgMCAxOTYuOTMgMzUiPjxyZWN0IGNsYXNzPSJzdmdfX3JlY3QiIHg9IjAiIHk9IjAiIHdpZHRoPSIxMTcuMDMiIGhlaWdodD0iMzUiIGZpbGw9IiNEQzU3NkQiLz48cmVjdCBjbGFzcz0ic3ZnX19yZWN0IiB4PSIxMTUuMDMiIHk9IjAiIHdpZHRoPSI4MS45IiBoZWlnaHQ9IjM1IiBmaWxsPSIjQzEzQjNBIi8+PHBhdGggY2xhc3M9InN2Z19fdGV4dCIgZD0iTTE3LjMzIDIyTDE0LjIyIDIyTDE0LjIyIDEzLjQ3TDE3LjE0IDEzLjQ3UTE4LjU5IDEzLjQ3IDE5LjM0IDE0LjA1UTIwLjEwIDE0LjYzIDIwLjEwIDE1Ljc4TDIwLjEwIDE1Ljc4UTIwLjEwIDE2LjM2IDE5Ljc4IDE2LjgzUTE5LjQ3IDE3LjMwIDE4Ljg2IDE3LjU2TDE4Ljg2IDE3LjU2UTE5LjU1IDE3Ljc1IDE5LjkzIDE4LjI2UTIwLjMxIDE4Ljc4IDIwLjMxIDE5LjUxTDIwLjMxIDE5LjUxUTIwLjMxIDIwLjcxIDE5LjUzIDIxLjM2UTE4Ljc2IDIyIDE3LjMzIDIyTDE3LjMzIDIyWk0xNS43MCAxOC4xNUwxNS43MCAyMC44MkwxNy4zNSAyMC44MlExOC4wNCAyMC44MiAxOC40NCAyMC40N1ExOC44MyAyMC4xMyAxOC44MyAxOS41MUwxOC44MyAxOS41MVExOC44MyAxOC4xOCAxNy40NyAxOC4xNUwxNy40NyAxOC4xNUwxNS43MCAxOC4xNVpNMTUuNzAgMTQuNjZMMTUuNzAgMTcuMDZMMTcuMTUgMTcuMDZRMTcuODQgMTcuMDYgMTguMjMgMTYuNzVRMTguNjIgMTYuNDMgMTguNjIgMTUuODZMMTguNjIgMTUuODZRMTguNjIgMTUuMjMgMTguMjYgMTQuOTVRMTcuOTAgMTQuNjYgMTcuMTQgMTQuNjZMMTcuMTQgMTQuNjZMMTUuNzAgMTQuNjZaTTI0LjY0IDE5LjE2TDI0LjY0IDE5LjE2TDI0LjY0IDEzLjQ3TDI2LjEyIDEzLjQ3TDI2LjEyIDE5LjE4UTI2LjEyIDIwLjAzIDI2LjU1IDIwLjQ4UTI2Ljk4IDIwLjkzIDI3LjgzIDIwLjkzTDI3LjgzIDIwLjkzUTI5LjU0IDIwLjkzIDI5LjU0IDE5LjEzTDI5LjU0IDE5LjEzTDI5LjU0IDEzLjQ3TDMxLjAyIDEzLjQ3TDMxLjAyIDE5LjE3UTMxLjAyIDIwLjUzIDMwLjE1IDIxLjMyUTI5LjI4IDIyLjEyIDI3LjgzIDIyLjEyTDI3LjgzIDIyLjEyUTI2LjM2IDIyLjEyIDI1LjUwIDIxLjMzUTI0LjY0IDIwLjU1IDI0LjY0IDE5LjE2Wk0zNy4xNSAyMkwzNS42NyAyMkwzNS42NyAxMy40N0wzNy4xNSAxMy40N0wzNy4xNSAyMlpNNDcuMzIgMjJMNDEuOTYgMjJMNDEuOTYgMTMuNDdMNDMuNDQgMTMuNDdMNDMuNDQgMjAuODJMNDcuMzIgMjAuODJMNDcuMzIgMjJaTTUzLjEyIDE0LjY2TDUwLjQ5IDE0LjY2TDUwLjQ5IDEzLjQ3TDU3LjI1IDEzLjQ3TDU3LjI1IDE0LjY2TDU0LjU5IDE0LjY2TDU0LjU5IDIyTDUzLjEyIDIyTDUzLjEyIDE0LjY2Wk02OC4zNyAyMkw2Ni40MCAxMy40N0w2Ny44NyAxMy40N0w2OS4yMCAxOS44OEw3MC44MiAxMy40N0w3Mi4wNyAxMy40N0w3My42OCAxOS44OUw3NC45OSAxMy40N0w3Ni40NiAxMy40N0w3NC40OSAyMkw3My4wNyAyMkw3MS40NSAxNS43N0w2OS43OSAyMkw2OC4zNyAyMlpNODIuMTAgMjJMODAuNjIgMjJMODAuNjIgMTMuNDdMODIuMTAgMTMuNDdMODIuMTAgMjJaTTg4LjU5IDE0LjY2TDg1Ljk1IDE0LjY2TDg1Ljk1IDEzLjQ3TDkyLjcyIDEzLjQ3TDkyLjcyIDE0LjY2TDkwLjA2IDE0LjY2TDkwLjA2IDIyTDg4LjU5IDIyTDg4LjU5IDE0LjY2Wk05Ny45NiAyMkw5Ni40OCAyMkw5Ni40OCAxMy40N0w5Ny45NiAxMy40N0w5Ny45NiAxNy4wMkwxMDEuNzcgMTcuMDJMMTAxLjc3IDEzLjQ3TDEwMy4yNSAxMy40N0wxMDMuMjUgMjJMMTAxLjc3IDIyTDEwMS43NyAxOC4yMUw5Ny45NiAxOC4yMUw5Ny45NiAyMloiIGZpbGw9IiNGRkZGRkYiLz48cGF0aCBjbGFzcz0ic3ZnX190ZXh0IiBkPSJNMTMxLjYwIDIyTDEyOS4yMiAyMkwxMjkuMjIgMTMuNjBMMTMzLjA2IDEzLjYwUTEzNC4yMCAxMy42MCAxMzUuMDQgMTMuOThRMTM1Ljg4IDE0LjM1IDEzNi4zNCAxNS4wNlExMzYuNzkgMTUuNzYgMTM2Ljc5IDE2LjcxTDEzNi43OSAxNi43MVExMzYuNzkgMTcuNjIgMTM2LjM3IDE4LjMwUTEzNS45NCAxOC45OCAxMzUuMTUgMTkuMzZMMTM1LjE1IDE5LjM2TDEzNi45NiAyMkwxMzQuNDIgMjJMMTMyLjg5IDE5Ljc3TDEzMS42MCAxOS43N0wxMzEuNjAgMjJaTTEzMS42MCAxNS40N0wxMzEuNjAgMTcuOTNMMTMyLjkyIDE3LjkzUTEzMy42NSAxNy45MyAxMzQuMDIgMTcuNjFRMTM0LjM5IDE3LjI5IDEzNC4zOSAxNi43MUwxMzQuMzkgMTYuNzFRMTM0LjM5IDE2LjEyIDEzNC4wMiAxNS43OVExMzMuNjUgMTUuNDcgMTMyLjkyIDE1LjQ3TDEzMi45MiAxNS40N0wxMzEuNjAgMTUuNDdaTTE0OC4zMyAyMkwxNDEuNTggMjJMMTQxLjU4IDEzLjYwTDE0OC4xNyAxMy42MEwxNDguMTcgMTUuNDRMMTQzLjk0IDE1LjQ0TDE0My45NCAxNi44NUwxNDcuNjcgMTYuODVMMTQ3LjY3IDE4LjYzTDE0My45NCAxOC42M0wxNDMuOTQgMjAuMTdMMTQ4LjMzIDIwLjE3TDE0OC4zMyAyMlpNMTU0LjU1IDIyTDE1Mi4xMiAyMkwxNTUuODMgMTMuNjBMMTU4LjE3IDEzLjYwTDE2MS44OSAyMkwxNTkuNDIgMjJMMTU4Ljc2IDIwLjM3TDE1NS4yMSAyMC4zN0wxNTQuNTUgMjJaTTE1Ni45OSAxNS45M0wxNTUuOTAgMTguNjFMMTU4LjA2IDE4LjYxTDE1Ni45OSAxNS45M1pNMTY1LjYyIDE3LjgwTDE2NS42MiAxNy44MFExNjUuNjIgMTYuNTQgMTY2LjIxIDE1LjU0UTE2Ni44MSAxNC41NSAxNjcuODYgMTMuOTlRMTY4LjkyIDEzLjQzIDE3MC4yMyAxMy40M0wxNzAuMjMgMTMuNDNRMTcxLjM5IDEzLjQzIDE3Mi4zMSAxMy44NFExNzMuMjMgMTQuMjUgMTczLjg1IDE1LjAyTDE3My44NSAxNS4wMkwxNzIuMzQgMTYuMzlRMTcxLjUyIDE1LjQwIDE3MC4zNiAxNS40MEwxNzAuMzYgMTUuNDBRMTY5LjY3IDE1LjQwIDE2OS4xNCAxNS43MFExNjguNjAgMTYgMTY4LjMxIDE2LjU0UTE2OC4wMSAxNy4wOSAxNjguMDEgMTcuODBMMTY4LjAxIDE3LjgwUTE2OC4wMSAxOC41MSAxNjguMzEgMTkuMDVRMTY4LjYwIDE5LjYwIDE2OS4xNCAxOS45MFExNjkuNjcgMjAuMjAgMTcwLjM2IDIwLjIwTDE3MC4zNiAyMC4yMFExNzEuNTIgMjAuMjAgMTcyLjM0IDE5LjIyTDE3Mi4zNCAxOS4yMkwxNzMuODUgMjAuNThRMTczLjI0IDIxLjM1IDE3Mi4zMSAyMS43NlExNzEuMzkgMjIuMTcgMTcwLjIzIDIyLjE3TDE3MC4yMyAyMi4xN1ExNjguOTIgMjIuMTcgMTY3Ljg2IDIxLjYxUTE2Ni44MSAyMS4wNSAxNjYuMjEgMjAuMDVRMTY1LjYyIDE5LjA2IDE2NS42MiAxNy44MFpNMTgwLjE4IDE1LjQ4TDE3Ny41OSAxNS40OEwxNzcuNTkgMTMuNjBMMTg1LjEyIDEzLjYwTDE4NS4xMiAxNS40OEwxODIuNTUgMTUuNDhMMTgyLjU1IDIyTDE4MC4xOCAyMkwxODAuMTggMTUuNDhaIiBmaWxsPSIjRUZFRkVGIiB4PSIxMjguMDMiLz48L3N2Zz4=)](https://forthebadge.com)

[![forthebadge](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIzMTYuMSIgaGVpZ2h0PSIzNSIgdmlld0JveD0iMCAwIDMxNi4xIDM1Ij48cmVjdCBjbGFzcz0ic3ZnX19yZWN0IiB4PSIwIiB5PSIwIiB3aWR0aD0iMTU5LjkxIiBoZWlnaHQ9IjM1IiBmaWxsPSIjMDA1Mzg0Ii8+PHJlY3QgY2xhc3M9InN2Z19fcmVjdCIgeD0iMTU3LjkxIiB5PSIwIiB3aWR0aD0iMTU4LjE5IiBoZWlnaHQ9IjM1IiBmaWxsPSIjNjNCNENGIi8+PHBhdGggY2xhc3M9InN2Z19fdGV4dCIgZD0iTTE2LjY3IDIyTDE0LjIyIDIyTDE0LjIyIDEzLjQ3TDE2Ljc0IDEzLjQ3UTE3Ljg3IDEzLjQ3IDE4Ljc0IDEzLjk3UTE5LjYyIDE0LjQ4IDIwLjEwIDE1LjQwUTIwLjU4IDE2LjMzIDIwLjU4IDE3LjUyTDIwLjU4IDE3LjUyTDIwLjU4IDE3Ljk1UTIwLjU4IDE5LjE2IDIwLjEwIDIwLjA4UTE5LjYxIDIxLjAwIDE4LjcyIDIxLjUwUTE3LjgzIDIyIDE2LjY3IDIyTDE2LjY3IDIyWk0xNS43MCAxNC42NkwxNS43MCAyMC44MkwxNi42NyAyMC44MlExNy44MyAyMC44MiAxOC40NiAyMC4wOVExOS4wOCAxOS4zNiAxOS4wOSAxNy45OUwxOS4wOSAxNy45OUwxOS4wOSAxNy41MlExOS4wOSAxNi4xMyAxOC40OSAxNS40MFExNy44OSAxNC42NiAxNi43NCAxNC42NkwxNi43NCAxNC42NkwxNS43MCAxNC42NlpNMzAuNjIgMjJMMjUuMDUgMjJMMjUuMDUgMTMuNDdMMzAuNTggMTMuNDdMMzAuNTggMTQuNjZMMjYuNTMgMTQuNjZMMjYuNTMgMTcuMDJMMzAuMDMgMTcuMDJMMzAuMDMgMTguMTlMMjYuNTMgMTguMTlMMjYuNTMgMjAuODJMMzAuNjIgMjAuODJMMzAuNjIgMjJaTTM0LjM5IDE5LjQyTDM0LjM5IDE5LjQyTDM1Ljg3IDE5LjQyUTM1Ljg3IDIwLjE1IDM2LjM1IDIwLjU1UTM2LjgzIDIwLjk1IDM3LjczIDIwLjk1TDM3LjczIDIwLjk1UTM4LjUwIDIwLjk1IDM4Ljg5IDIwLjYzUTM5LjI4IDIwLjMyIDM5LjI4IDE5LjgwTDM5LjI4IDE5LjgwUTM5LjI4IDE5LjI0IDM4Ljg4IDE4Ljk0UTM4LjQ5IDE4LjYzIDM3LjQ2IDE4LjMyUTM2LjQyIDE4LjAxIDM1LjgxIDE3LjYzTDM1LjgxIDE3LjYzUTM0LjY1IDE2LjkwIDM0LjY1IDE1LjcyTDM0LjY1IDE1LjcyUTM0LjY1IDE0LjY5IDM1LjQ5IDE0LjAyUTM2LjMzIDEzLjM1IDM3LjY3IDEzLjM1TDM3LjY3IDEzLjM1UTM4LjU2IDEzLjM1IDM5LjI2IDEzLjY4UTM5Ljk2IDE0LjAxIDQwLjM2IDE0LjYxUTQwLjc1IDE1LjIyIDQwLjc1IDE1Ljk2TDQwLjc1IDE1Ljk2TDM5LjI4IDE1Ljk2UTM5LjI4IDE1LjI5IDM4Ljg2IDE0LjkxUTM4LjQ0IDE0LjU0IDM3LjY2IDE0LjU0TDM3LjY2IDE0LjU0UTM2LjkzIDE0LjU0IDM2LjUzIDE0Ljg1UTM2LjEzIDE1LjE2IDM2LjEzIDE1LjcxTDM2LjEzIDE1LjcxUTM2LjEzIDE2LjE4IDM2LjU2IDE2LjUwUTM3LjAwIDE2LjgxIDM3Ljk5IDE3LjEwUTM4Ljk5IDE3LjQwIDM5LjU5IDE3Ljc4UTQwLjIwIDE4LjE2IDQwLjQ4IDE4LjY1UTQwLjc2IDE5LjEzIDQwLjc2IDE5Ljc5TDQwLjc2IDE5Ljc5UTQwLjc2IDIwLjg2IDM5Ljk0IDIxLjQ5UTM5LjEzIDIyLjEyIDM3LjczIDIyLjEyTDM3LjczIDIyLjEyUTM2LjgwIDIyLjEyIDM2LjAyIDIxLjc3UTM1LjI1IDIxLjQzIDM0LjgyIDIwLjgzUTM0LjM5IDIwLjIyIDM0LjM5IDE5LjQyWk00Ni42MSAyMkw0NS4xNCAyMkw0NS4xNCAxMy40N0w0Ni42MSAxMy40N0w0Ni42MSAyMlpNNTEuMTggMTguMTNMNTEuMTggMTguMTNMNTEuMTggMTcuNDZRNTEuMTggMTUuNTMgNTIuMTAgMTQuNDRRNTMuMDMgMTMuMzUgNTQuNjkgMTMuMzVMNTQuNjkgMTMuMzVRNTYuMTEgMTMuMzUgNTYuOTUgMTQuMDVRNTcuNzkgMTQuNzYgNTcuOTYgMTYuMDhMNTcuOTYgMTYuMDhMNTYuNTAgMTYuMDhRNTYuMjYgMTQuNTQgNTQuNzIgMTQuNTRMNTQuNzIgMTQuNTRRNTMuNzIgMTQuNTQgNTMuMjAgMTUuMjZRNTIuNjggMTUuOTggNTIuNjcgMTcuMzdMNTIuNjcgMTcuMzdMNTIuNjcgMTguMDJRNTIuNjcgMTkuNDAgNTMuMjUgMjAuMTdRNTMuODMgMjAuOTMgNTQuODcgMjAuOTNMNTQuODcgMjAuOTNRNTYuMDEgMjAuOTMgNTYuNDkgMjAuNDJMNTYuNDkgMjAuNDJMNTYuNDkgMTguNzVMNTQuNzMgMTguNzVMNTQuNzMgMTcuNjJMNTcuOTYgMTcuNjJMNTcuOTYgMjAuODlRNTcuNTAgMjEuNTAgNTYuNjggMjEuODFRNTUuODYgMjIuMTIgNTQuODIgMjIuMTJMNTQuODIgMjIuMTJRNTMuNzQgMjIuMTIgNTIuOTIgMjEuNjNRNTIuMDkgMjEuMTQgNTEuNjQgMjAuMjRRNTEuMjAgMTkuMzMgNTEuMTggMTguMTNaTTY0LjA2IDIyTDYyLjU4IDIyTDYyLjU4IDEzLjQ3TDY0LjA2IDEzLjQ3TDY3Ljg4IDE5LjU0TDY3Ljg4IDEzLjQ3TDY5LjM1IDEzLjQ3TDY5LjM1IDIyTDY3Ljg3IDIyTDY0LjA2IDE1Ljk1TDY0LjA2IDIyWk03OS42NyAyMkw3NC4wOSAyMkw3NC4wOSAxMy40N0w3OS42MyAxMy40N0w3OS42MyAxNC42Nkw3NS41NyAxNC42Nkw3NS41NyAxNy4wMkw3OS4wNyAxNy4wMkw3OS4wNyAxOC4xOUw3NS41NyAxOC4xOUw3NS41NyAyMC44Mkw3OS42NyAyMC44Mkw3OS42NyAyMlpNODYuMzIgMjJMODMuODYgMjJMODMuODYgMTMuNDdMODYuMzggMTMuNDdRODcuNTEgMTMuNDcgODguMzkgMTMuOTdRODkuMjYgMTQuNDggODkuNzQgMTUuNDBROTAuMjIgMTYuMzMgOTAuMjIgMTcuNTJMOTAuMjIgMTcuNTJMOTAuMjIgMTcuOTVROTAuMjIgMTkuMTYgODkuNzQgMjAuMDhRODkuMjYgMjEuMDAgODguMzYgMjEuNTBRODcuNDcgMjIgODYuMzIgMjJMODYuMzIgMjJaTTg1LjM0IDE0LjY2TDg1LjM0IDIwLjgyTDg2LjMxIDIwLjgyUTg3LjQ4IDIwLjgyIDg4LjEwIDIwLjA5UTg4LjcyIDE5LjM2IDg4Ljc0IDE3Ljk5TDg4Ljc0IDE3Ljk5TDg4Ljc0IDE3LjUyUTg4Ljc0IDE2LjEzIDg4LjEzIDE1LjQwUTg3LjUzIDE0LjY2IDg2LjM4IDE0LjY2TDg2LjM4IDE0LjY2TDg1LjM0IDE0LjY2Wk0xMDAuNTMgMTkuMTZMMTAwLjUzIDE5LjE2TDEwMC41MyAxMy40N0wxMDIuMDEgMTMuNDdMMTAyLjAxIDE5LjE4UTEwMi4wMSAyMC4wMyAxMDIuNDQgMjAuNDhRMTAyLjg4IDIwLjkzIDEwMy43MiAyMC45M0wxMDMuNzIgMjAuOTNRMTA1LjQzIDIwLjkzIDEwNS40MyAxOS4xM0wxMDUuNDMgMTkuMTNMMTA1LjQzIDEzLjQ3TDEwNi45MSAxMy40N0wxMDYuOTEgMTkuMTdRMTA2LjkxIDIwLjUzIDEwNi4wNCAyMS4zMlExMDUuMTcgMjIuMTIgMTAzLjcyIDIyLjEyTDEwMy43MiAyMi4xMlExMDIuMjUgMjIuMTIgMTAxLjM5IDIxLjMzUTEwMC41MyAyMC41NSAxMDAuNTMgMTkuMTZaTTExMS4wNCAxOS40MkwxMTEuMDQgMTkuNDJMMTEyLjUzIDE5LjQyUTExMi41MyAyMC4xNSAxMTMuMDEgMjAuNTVRMTEzLjQ5IDIwLjk1IDExNC4zOCAyMC45NUwxMTQuMzggMjAuOTVRMTE1LjE2IDIwLjk1IDExNS41NSAyMC42M1ExMTUuOTQgMjAuMzIgMTE1Ljk0IDE5LjgwTDExNS45NCAxOS44MFExMTUuOTQgMTkuMjQgMTE1LjU0IDE4Ljk0UTExNS4xNCAxOC42MyAxMTQuMTEgMTguMzJRMTEzLjA4IDE4LjAxIDExMi40NyAxNy42M0wxMTIuNDcgMTcuNjNRMTExLjMxIDE2LjkwIDExMS4zMSAxNS43MkwxMTEuMzEgMTUuNzJRMTExLjMxIDE0LjY5IDExMi4xNSAxNC4wMlExMTIuOTkgMTMuMzUgMTE0LjMzIDEzLjM1TDExNC4zMyAxMy4zNVExMTUuMjIgMTMuMzUgMTE1LjkyIDEzLjY4UTExNi42MiAxNC4wMSAxMTcuMDEgMTQuNjFRMTE3LjQxIDE1LjIyIDExNy40MSAxNS45NkwxMTcuNDEgMTUuOTZMMTE1Ljk0IDE1Ljk2UTExNS45NCAxNS4yOSAxMTUuNTIgMTQuOTFRMTE1LjEwIDE0LjU0IDExNC4zMiAxNC41NEwxMTQuMzIgMTQuNTRRMTEzLjU5IDE0LjU0IDExMy4xOSAxNC44NVExMTIuNzkgMTUuMTYgMTEyLjc5IDE1LjcxTDExMi43OSAxNS43MVExMTIuNzkgMTYuMTggMTEzLjIyIDE2LjUwUTExMy42NiAxNi44MSAxMTQuNjUgMTcuMTBRMTE1LjY1IDE3LjQwIDExNi4yNSAxNy43OFExMTYuODYgMTguMTYgMTE3LjE0IDE4LjY1UTExNy40MiAxOS4xMyAxMTcuNDIgMTkuNzlMMTE3LjQyIDE5Ljc5UTExNy40MiAyMC44NiAxMTYuNjAgMjEuNDlRMTE1Ljc4IDIyLjEyIDExNC4zOCAyMi4xMkwxMTQuMzggMjIuMTJRMTEzLjQ2IDIyLjEyIDExMi42OCAyMS43N1ExMTEuOTAgMjEuNDMgMTExLjQ3IDIwLjgzUTExMS4wNCAyMC4yMiAxMTEuMDQgMTkuNDJaTTEyMy4yNyAyMkwxMjEuODAgMjJMMTIxLjgwIDEzLjQ3TDEyMy4yNyAxMy40N0wxMjMuMjcgMjJaTTEyOS41NiAyMkwxMjguMDggMjJMMTI4LjA4IDEzLjQ3TDEyOS41NiAxMy40N0wxMzMuMzggMTkuNTRMMTMzLjM4IDEzLjQ3TDEzNC44NSAxMy40N0wxMzQuODUgMjJMMTMzLjM3IDIyTDEyOS41NiAxNS45NUwxMjkuNTYgMjJaTTEzOS4zNCAxOC4xM0wxMzkuMzQgMTguMTNMMTM5LjM0IDE3LjQ2UTEzOS4zNCAxNS41MyAxNDAuMjcgMTQuNDRRMTQxLjIwIDEzLjM1IDE0Mi44NSAxMy4zNUwxNDIuODUgMTMuMzVRMTQ0LjI4IDEzLjM1IDE0NS4xMiAxNC4wNVExNDUuOTUgMTQuNzYgMTQ2LjEyIDE2LjA4TDE0Ni4xMiAxNi4wOEwxNDQuNjcgMTYuMDhRMTQ0LjQyIDE0LjU0IDE0Mi44OCAxNC41NEwxNDIuODggMTQuNTRRMTQxLjg5IDE0LjU0IDE0MS4zNyAxNS4yNlExNDAuODUgMTUuOTggMTQwLjgzIDE3LjM3TDE0MC44MyAxNy4zN0wxNDAuODMgMTguMDJRMTQwLjgzIDE5LjQwIDE0MS40MiAyMC4xN1ExNDIuMDAgMjAuOTMgMTQzLjA0IDIwLjkzTDE0My4wNCAyMC45M1ExNDQuMTcgMjAuOTMgMTQ0LjY1IDIwLjQyTDE0NC42NSAyMC40MkwxNDQuNjUgMTguNzVMMTQyLjg5IDE4Ljc1TDE0Mi44OSAxNy42MkwxNDYuMTMgMTcuNjJMMTQ2LjEzIDIwLjg5UTE0NS42NyAyMS41MCAxNDQuODUgMjEuODFRMTQ0LjAzIDIyLjEyIDE0Mi45OCAyMi4xMkwxNDIuOTggMjIuMTJRMTQxLjkxIDIyLjEyIDE0MS4wOCAyMS42M1ExNDAuMjYgMjEuMTQgMTM5LjgxIDIwLjI0UTEzOS4zNiAxOS4zMyAxMzkuMzQgMTguMTNaIiBmaWxsPSIjRkZGRkZGIi8+PHBhdGggY2xhc3M9InN2Z19fdGV4dCIgZD0iTTE3My44OSAxNS40OEwxNzEuMzEgMTUuNDhMMTcxLjMxIDEzLjYwTDE3OC44MyAxMy42MEwxNzguODMgMTUuNDhMMTc2LjI2IDE1LjQ4TDE3Ni4yNiAyMkwxNzMuODkgMjJMMTczLjg5IDE1LjQ4Wk0xODQuNjIgMjJMMTgyLjE5IDIyTDE4NS45MCAxMy42MEwxODguMjUgMTMuNjBMMTkxLjk2IDIyTDE4OS40OSAyMkwxODguODMgMjAuMzdMMTg1LjI4IDIwLjM3TDE4NC42MiAyMlpNMTg3LjA2IDE1LjkzTDE4NS45NyAxOC42MUwxODguMTMgMTguNjFMMTg3LjA2IDE1LjkzWk0xOTguNDkgMjJMMTk2LjEyIDIyTDE5Ni4xMiAxMy42MEwxOTguNDkgMTMuNjBMMTk4LjQ5IDIyWk0yMTAuMDUgMjJMMjAzLjY3IDIyTDIwMy42NyAxMy42MEwyMDYuMDUgMTMuNjBMMjA2LjA1IDIwLjExTDIxMC4wNSAyMC4xMUwyMTAuMDUgMjJaTTIxNi41NSAyMkwyMTMuODMgMTMuNjBMMjE2LjI4IDEzLjYwTDIxNy45NyAxOC45NkwyMTkuNzQgMTMuNjBMMjIxLjkzIDEzLjYwTDIyMy42MiAxOS4wMUwyMjUuMzggMTMuNjBMMjI3LjY1IDEzLjYwTDIyNC45MyAyMkwyMjIuMzggMjJMMjIwLjc4IDE2Ljg5TDIxOS4xMCAyMkwyMTYuNTUgMjJaTTIzNC41NCAyMkwyMzIuMTYgMjJMMjMyLjE2IDEzLjYwTDIzNC41NCAxMy42MEwyMzQuNTQgMjJaTTI0Mi4wNSAyMkwyMzkuNzIgMjJMMjM5LjcyIDEzLjYwTDI0MS42NyAxMy42MEwyNDUuMzggMTguMDdMMjQ1LjM4IDEzLjYwTDI0Ny43MSAxMy42MEwyNDcuNzEgMjJMMjQ1Ljc2IDIyTDI0Mi4wNSAxNy41MkwyNDIuMDUgMjJaTTI1Ni44NCAyMkwyNTIuODcgMjJMMjUyLjg3IDEzLjYwTDI1Ni44NCAxMy42MFEyNTguMjIgMTMuNjAgMjU5LjI5IDE0LjEyUTI2MC4zNiAxNC42MyAyNjAuOTUgMTUuNThRMjYxLjU0IDE2LjUzIDI2MS41NCAxNy44MEwyNjEuNTQgMTcuODBRMjYxLjU0IDE5LjA3IDI2MC45NSAyMC4wMlEyNjAuMzYgMjAuOTcgMjU5LjI5IDIxLjQ4UTI1OC4yMiAyMiAyNTYuODQgMjJMMjU2Ljg0IDIyWk0yNTUuMjUgMTUuNTBMMjU1LjI1IDIwLjEwTDI1Ni43NSAyMC4xMFEyNTcuODMgMjAuMTAgMjU4LjQ4IDE5LjQ5UTI1OS4xMyAxOC44OCAyNTkuMTMgMTcuODBMMjU5LjEzIDE3LjgwUTI1OS4xMyAxNi43MiAyNTguNDggMTYuMTFRMjU3LjgzIDE1LjUwIDI1Ni43NSAxNS41MEwyNTYuNzUgMTUuNTBMMjU1LjI1IDE1LjUwWk0yNzIuODEgMTcuODBMMjcyLjgxIDE3LjgwUTI3Mi44MSAxNi41NCAyNzMuNDEgMTUuNTRRMjc0LjAwIDE0LjU1IDI3NS4wNiAxMy45OVEyNzYuMTEgMTMuNDMgMjc3LjQzIDEzLjQzTDI3Ny40MyAxMy40M1EyNzguNTggMTMuNDMgMjc5LjUwIDEzLjg0UTI4MC40MyAxNC4yNSAyODEuMDQgMTUuMDJMMjgxLjA0IDE1LjAyTDI3OS41MyAxNi4zOVEyNzguNzIgMTUuNDAgMjc3LjU1IDE1LjQwTDI3Ny41NSAxNS40MFEyNzYuODYgMTUuNDAgMjc2LjMzIDE1LjcwUTI3NS44MCAxNiAyNzUuNTAgMTYuNTRRMjc1LjIxIDE3LjA5IDI3NS4yMSAxNy44MEwyNzUuMjEgMTcuODBRMjc1LjIxIDE4LjUxIDI3NS41MCAxOS4wNVEyNzUuODAgMTkuNjAgMjc2LjMzIDE5LjkwUTI3Ni44NiAyMC4yMCAyNzcuNTUgMjAuMjBMMjc3LjU1IDIwLjIwUTI3OC43MiAyMC4yMCAyNzkuNTMgMTkuMjJMMjc5LjUzIDE5LjIyTDI4MS4wNCAyMC41OFEyODAuNDMgMjEuMzUgMjc5LjUxIDIxLjc2UTI3OC41OCAyMi4xNyAyNzcuNDMgMjIuMTdMMjc3LjQzIDIyLjE3UTI3Ni4xMSAyMi4xNyAyNzUuMDYgMjEuNjFRMjc0LjAwIDIxLjA1IDI3My40MSAyMC4wNVEyNzIuODEgMTkuMDYgMjcyLjgxIDE3LjgwWk0yODQuOTkgMjEuMjRMMjg0Ljk5IDIxLjI0TDI4NS43NyAxOS40OVEyODYuMzMgMTkuODYgMjg3LjA4IDIwLjA5UTI4Ny44MiAyMC4zMiAyODguNTQgMjAuMzJMMjg4LjU0IDIwLjMyUTI4OS45MSAyMC4zMiAyODkuOTEgMTkuNjRMMjg5LjkxIDE5LjY0UTI4OS45MSAxOS4yOCAyODkuNTIgMTkuMTFRMjg5LjEzIDE4LjkzIDI4OC4yNyAxOC43NEwyODguMjcgMTguNzRRMjg3LjMyIDE4LjUzIDI4Ni42OCAxOC4zMFEyODYuMDUgMTguMDYgMjg1LjU5IDE3LjU1UTI4NS4xNCAxNy4wMyAyODUuMTQgMTYuMTZMMjg1LjE0IDE2LjE2UTI4NS4xNCAxNS4zOSAyODUuNTYgMTQuNzdRMjg1Ljk3IDE0LjE1IDI4Ni44MSAxMy43OVEyODcuNjQgMTMuNDMgMjg4Ljg1IDEzLjQzTDI4OC44NSAxMy40M1EyODkuNjggMTMuNDMgMjkwLjQ4IDEzLjYyUTI5MS4yOSAxMy44MCAyOTEuOTAgMTQuMTdMMjkxLjkwIDE0LjE3TDI5MS4xNyAxNS45M1EyODkuOTcgMTUuMjggMjg4Ljg0IDE1LjI4TDI4OC44NCAxNS4yOFEyODguMTMgMTUuMjggMjg3LjgxIDE1LjQ5UTI4Ny40OSAxNS43MCAyODcuNDkgMTYuMDRMMjg3LjQ5IDE2LjA0UTI4Ny40OSAxNi4zNyAyODcuODcgMTYuNTRRMjg4LjI1IDE2LjcxIDI4OS4xMCAxNi44OUwyODkuMTAgMTYuODlRMjkwLjA2IDE3LjEwIDI5MC42OSAxNy4zM1EyOTEuMzIgMTcuNTYgMjkxLjc5IDE4LjA3UTI5Mi4yNSAxOC41OCAyOTIuMjUgMTkuNDZMMjkyLjI1IDE5LjQ2UTI5Mi4yNSAyMC4yMSAyOTEuODMgMjAuODNRMjkxLjQxIDIxLjQ0IDI5MC41NyAyMS44MFEyODkuNzMgMjIuMTcgMjg4LjUzIDIyLjE3TDI4OC41MyAyMi4xN1EyODcuNTEgMjIuMTcgMjg2LjU1IDIxLjkyUTI4NS41OSAyMS42NyAyODQuOTkgMjEuMjRaTTI5Ni4yNCAyMS4yNEwyOTYuMjQgMjEuMjRMMjk3LjAyIDE5LjQ5UTI5Ny41OCAxOS44NiAyOTguMzMgMjAuMDlRMjk5LjA3IDIwLjMyIDI5OS43OSAyMC4zMkwyOTkuNzkgMjAuMzJRMzAxLjE2IDIwLjMyIDMwMS4xNiAxOS42NEwzMDEuMTYgMTkuNjRRMzAxLjE2IDE5LjI4IDMwMC43NyAxOS4xMVEzMDAuMzggMTguOTMgMjk5LjUyIDE4Ljc0TDI5OS41MiAxOC43NFEyOTguNTcgMTguNTMgMjk3LjkzIDE4LjMwUTI5Ny4zMCAxOC4wNiAyOTYuODQgMTcuNTVRMjk2LjM5IDE3LjAzIDI5Ni4zOSAxNi4xNkwyOTYuMzkgMTYuMTZRMjk2LjM5IDE1LjM5IDI5Ni44MSAxNC43N1EyOTcuMjIgMTQuMTUgMjk4LjA2IDEzLjc5UTI5OC44OSAxMy40MyAzMDAuMTAgMTMuNDNMMzAwLjEwIDEzLjQzUTMwMC45MyAxMy40MyAzMDEuNzMgMTMuNjJRMzAyLjU0IDEzLjgwIDMwMy4xNSAxNC4xN0wzMDMuMTUgMTQuMTdMMzAyLjQyIDE1LjkzUTMwMS4yMiAxNS4yOCAzMDAuMDkgMTUuMjhMMzAwLjA5IDE1LjI4UTI5OS4zOCAxNS4yOCAyOTkuMDYgMTUuNDlRMjk4Ljc0IDE1LjcwIDI5OC43NCAxNi4wNEwyOTguNzQgMTYuMDRRMjk4Ljc0IDE2LjM3IDI5OS4xMiAxNi41NFEyOTkuNTAgMTYuNzEgMzAwLjM1IDE2Ljg5TDMwMC4zNSAxNi44OVEzMDEuMzEgMTcuMTAgMzAxLjk0IDE3LjMzUTMwMi41NyAxNy41NiAzMDMuMDQgMTguMDdRMzAzLjUwIDE4LjU4IDMwMy41MCAxOS40NkwzMDMuNTAgMTkuNDZRMzAzLjUwIDIwLjIxIDMwMy4wOCAyMC44M1EzMDIuNjYgMjEuNDQgMzAxLjgyIDIxLjgwUTMwMC45OCAyMi4xNyAyOTkuNzggMjIuMTdMMjk5Ljc4IDIyLjE3UTI5OC43NiAyMi4xNyAyOTcuODAgMjEuOTJRMjk2Ljg0IDIxLjY3IDI5Ni4yNCAyMS4yNFoiIGZpbGw9IiNGRkZGRkYiIHg9IjE3MC45MSIvPjwvc3ZnPg==)](https://forthebadge.com)

[![forthebadge](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMzcuNDgwMDAwMDAwMDAwMDIiIGhlaWdodD0iMzUiIHZpZXdCb3g9IjAgMCAyMzcuNDgwMDAwMDAwMDAwMDIgMzUiPjxyZWN0IGNsYXNzPSJzdmdfX3JlY3QiIHg9IjAiIHk9IjAiIHdpZHRoPSIxMDguMDUiIGhlaWdodD0iMzUiIGZpbGw9IiM1RDk3NDEiLz48cmVjdCBjbGFzcz0ic3ZnX19yZWN0IiB4PSIxMDYuMDUiIHk9IjAiIHdpZHRoPSIxMzEuNDMiIGhlaWdodD0iMzUiIGZpbGw9IiM4RkM5NjUiLz48cGF0aCBjbGFzcz0ic3ZnX190ZXh0IiBkPSJNMTMuNzggMTkuNDJMMTMuNzggMTkuNDJMMTUuMjcgMTkuNDJRMTUuMjcgMjAuMTUgMTUuNzUgMjAuNTVRMTYuMjMgMjAuOTUgMTcuMTIgMjAuOTVMMTcuMTIgMjAuOTVRMTcuOTAgMjAuOTUgMTguMjkgMjAuNjNRMTguNjggMjAuMzIgMTguNjggMTkuODBMMTguNjggMTkuODBRMTguNjggMTkuMjQgMTguMjggMTguOTRRMTcuODkgMTguNjMgMTYuODUgMTguMzJRMTUuODIgMTguMDEgMTUuMjEgMTcuNjNMMTUuMjEgMTcuNjNRMTQuMDUgMTYuOTAgMTQuMDUgMTUuNzJMMTQuMDUgMTUuNzJRMTQuMDUgMTQuNjkgMTQuODkgMTQuMDJRMTUuNzMgMTMuMzUgMTcuMDcgMTMuMzVMMTcuMDcgMTMuMzVRMTcuOTYgMTMuMzUgMTguNjYgMTMuNjhRMTkuMzYgMTQuMDEgMTkuNzUgMTQuNjFRMjAuMTUgMTUuMjIgMjAuMTUgMTUuOTZMMjAuMTUgMTUuOTZMMTguNjggMTUuOTZRMTguNjggMTUuMjkgMTguMjYgMTQuOTFRMTcuODQgMTQuNTQgMTcuMDYgMTQuNTRMMTcuMDYgMTQuNTRRMTYuMzMgMTQuNTQgMTUuOTMgMTQuODVRMTUuNTMgMTUuMTYgMTUuNTMgMTUuNzFMMTUuNTMgMTUuNzFRMTUuNTMgMTYuMTggMTUuOTYgMTYuNTBRMTYuNDAgMTYuODEgMTcuMzkgMTcuMTBRMTguMzkgMTcuNDAgMTguOTkgMTcuNzhRMTkuNjAgMTguMTYgMTkuODggMTguNjVRMjAuMTYgMTkuMTMgMjAuMTYgMTkuNzlMMjAuMTYgMTkuNzlRMjAuMTYgMjAuODYgMTkuMzQgMjEuNDlRMTguNTIgMjIuMTIgMTcuMTIgMjIuMTJMMTcuMTIgMjIuMTJRMTYuMjAgMjIuMTIgMTUuNDIgMjEuNzdRMTQuNjQgMjEuNDMgMTQuMjEgMjAuODNRMTMuNzggMjAuMjIgMTMuNzggMTkuNDJaTTI0LjMxIDE5LjE2TDI0LjMxIDE5LjE2TDI0LjMxIDEzLjQ3TDI1Ljc5IDEzLjQ3TDI1Ljc5IDE5LjE4UTI1Ljc5IDIwLjAzIDI2LjIyIDIwLjQ4UTI2LjY2IDIwLjkzIDI3LjUwIDIwLjkzTDI3LjUwIDIwLjkzUTI5LjIxIDIwLjkzIDI5LjIxIDE5LjEzTDI5LjIxIDE5LjEzTDI5LjIxIDEzLjQ3TDMwLjY5IDEzLjQ3TDMwLjY5IDE5LjE3UTMwLjY5IDIwLjUzIDI5LjgyIDIxLjMyUTI4Ljk1IDIyLjEyIDI3LjUwIDIyLjEyTDI3LjUwIDIyLjEyUTI2LjA0IDIyLjEyIDI1LjE3IDIxLjMzUTI0LjMxIDIwLjU1IDI0LjMxIDE5LjE2Wk0zNi43NCAyMkwzNS4yNiAyMkwzNS4yNiAxMy40N0wzOC41MiAxMy40N1EzOS45NSAxMy40NyA0MC43OSAxNC4yMVE0MS42MyAxNC45NiA0MS42MyAxNi4xOEw0MS42MyAxNi4xOFE0MS42MyAxNy40NCA0MC44MSAxOC4xM1EzOS45OSAxOC44MyAzOC41MCAxOC44M0wzOC41MCAxOC44M0wzNi43NCAxOC44M0wzNi43NCAyMlpNMzYuNzQgMTQuNjZMMzYuNzQgMTcuNjRMMzguNTIgMTcuNjRRMzkuMzEgMTcuNjQgMzkuNzMgMTcuMjdRNDAuMTQgMTYuOTAgNDAuMTQgMTYuMTlMNDAuMTQgMTYuMTlRNDAuMTQgMTUuNTAgMzkuNzIgMTUuMDlRMzkuMzAgMTQuNjggMzguNTYgMTQuNjZMMzguNTYgMTQuNjZMMzYuNzQgMTQuNjZaTTQ3LjQwIDIyTDQ1LjkyIDIyTDQ1LjkyIDEzLjQ3TDQ5LjE4IDEzLjQ3UTUwLjYxIDEzLjQ3IDUxLjQ1IDE0LjIxUTUyLjI5IDE0Ljk2IDUyLjI5IDE2LjE4TDUyLjI5IDE2LjE4UTUyLjI5IDE3LjQ0IDUxLjQ3IDE4LjEzUTUwLjY0IDE4LjgzIDQ5LjE2IDE4LjgzTDQ5LjE2IDE4LjgzTDQ3LjQwIDE4LjgzTDQ3LjQwIDIyWk00Ny40MCAxNC42Nkw0Ny40MCAxNy42NEw0OS4xOCAxNy42NFE0OS45NyAxNy42NCA1MC4zOSAxNy4yN1E1MC44MCAxNi45MCA1MC44MCAxNi4xOUw1MC44MCAxNi4xOVE1MC44MCAxNS41MCA1MC4zOCAxNS4wOVE0OS45NiAxNC42OCA0OS4yMiAxNC42Nkw0OS4yMiAxNC42Nkw0Ny40MCAxNC42NlpNNTYuMzEgMTguMDBMNTYuMzEgMTguMDBMNTYuMzEgMTcuNTJRNTYuMzEgMTYuMjggNTYuNzUgMTUuMzJRNTcuMTkgMTQuMzcgNTguMDAgMTMuODZRNTguODAgMTMuMzUgNTkuODQgMTMuMzVRNjAuODkgMTMuMzUgNjEuNjkgMTMuODVRNjIuNTAgMTQuMzUgNjIuOTQgMTUuMjlRNjMuMzggMTYuMjMgNjMuMzggMTcuNDhMNjMuMzggMTcuNDhMNjMuMzggMTcuOTZRNjMuMzggMTkuMjEgNjIuOTUgMjAuMTZRNjIuNTIgMjEuMTAgNjEuNzEgMjEuNjFRNjAuOTAgMjIuMTIgNTkuODYgMjIuMTJMNTkuODYgMjIuMTJRNTguODIgMjIuMTIgNTguMDEgMjEuNjFRNTcuMjAgMjEuMTAgNTYuNzUgMjAuMTdRNTYuMzEgMTkuMjMgNTYuMzEgMTguMDBaTTU3Ljc5IDE3LjQ2TDU3Ljc5IDE3Ljk2UTU3Ljc5IDE5LjM2IDU4LjM0IDIwLjEzUTU4Ljg4IDIwLjkwIDU5Ljg2IDIwLjkwTDU5Ljg2IDIwLjkwUTYwLjg0IDIwLjkwIDYxLjM3IDIwLjE1UTYxLjkwIDE5LjQwIDYxLjkwIDE3Ljk2TDYxLjkwIDE3Ljk2TDYxLjkwIDE3LjUxUTYxLjkwIDE2LjA5IDYxLjM2IDE1LjM0UTYwLjgzIDE0LjU4IDU5Ljg0IDE0LjU4TDU5Ljg0IDE0LjU4UTU4Ljg4IDE0LjU4IDU4LjM0IDE1LjMzUTU3LjgwIDE2LjA5IDU3Ljc5IDE3LjQ2TDU3Ljc5IDE3LjQ2Wk02OS4zMyAyMkw2Ny44NSAyMkw2Ny44NSAxMy40N0w3MC44NSAxMy40N1E3Mi4zMiAxMy40NyA3My4xMyAxNC4xM1E3My45MyAxNC43OSA3My45MyAxNi4wNUw3My45MyAxNi4wNVE3My45MyAxNi45MCA3My41MiAxNy40OFE3My4xMCAxOC4wNiA3Mi4zNyAxOC4zN0w3Mi4zNyAxOC4zN0w3NC4yOCAyMS45Mkw3NC4yOCAyMkw3Mi42OSAyMkw3MC45OCAxOC43MUw2OS4zMyAxOC43MUw2OS4zMyAyMlpNNjkuMzMgMTQuNjZMNjkuMzMgMTcuNTJMNzAuODUgMTcuNTJRNzEuNjAgMTcuNTIgNzIuMDMgMTcuMTVRNzIuNDUgMTYuNzcgNzIuNDUgMTYuMTFMNzIuNDUgMTYuMTFRNzIuNDUgMTUuNDMgNzIuMDYgMTUuMDVRNzEuNjcgMTQuNjggNzAuODkgMTQuNjZMNzAuODkgMTQuNjZMNjkuMzMgMTQuNjZaTTgwLjAxIDE0LjY2TDc3LjM3IDE0LjY2TDc3LjM3IDEzLjQ3TDg0LjE0IDEzLjQ3TDg0LjE0IDE0LjY2TDgxLjQ4IDE0LjY2TDgxLjQ4IDIyTDgwLjAxIDIyTDgwLjAxIDE0LjY2Wk04Ny40NiAxOS40Mkw4Ny40NiAxOS40Mkw4OC45NCAxOS40MlE4OC45NCAyMC4xNSA4OS40MiAyMC41NVE4OS45MCAyMC45NSA5MC44MCAyMC45NUw5MC44MCAyMC45NVE5MS41NyAyMC45NSA5MS45NiAyMC42M1E5Mi4zNSAyMC4zMiA5Mi4zNSAxOS44MEw5Mi4zNSAxOS44MFE5Mi4zNSAxOS4yNCA5MS45NiAxOC45NFE5MS41NiAxOC42MyA5MC41MyAxOC4zMlE4OS41MCAxOC4wMSA4OC44OSAxNy42M0w4OC44OSAxNy42M1E4Ny43MiAxNi45MCA4Ny43MiAxNS43Mkw4Ny43MiAxNS43MlE4Ny43MiAxNC42OSA4OC41NiAxNC4wMlE4OS40MCAxMy4zNSA5MC43NSAxMy4zNUw5MC43NSAxMy4zNVE5MS42NCAxMy4zNSA5Mi4zMyAxMy42OFE5My4wMyAxNC4wMSA5My40MyAxNC42MVE5My44MyAxNS4yMiA5My44MyAxNS45Nkw5My44MyAxNS45Nkw5Mi4zNSAxNS45NlE5Mi4zNSAxNS4yOSA5MS45MyAxNC45MVE5MS41MSAxNC41NCA5MC43MyAxNC41NEw5MC43MyAxNC41NFE5MC4wMSAxNC41NCA4OS42MSAxNC44NVE4OS4yMSAxNS4xNiA4OS4yMSAxNS43MUw4OS4yMSAxNS43MVE4OS4yMSAxNi4xOCA4OS42NCAxNi41MFE5MC4wNyAxNi44MSA5MS4wNyAxNy4xMFE5Mi4wNiAxNy40MCA5Mi42NyAxNy43OFE5My4yNyAxOC4xNiA5My41NSAxOC42NVE5My44MyAxOS4xMyA5My44MyAxOS43OUw5My44MyAxOS43OVE5My44MyAyMC44NiA5My4wMiAyMS40OVE5Mi4yMCAyMi4xMiA5MC44MCAyMi4xMkw5MC44MCAyMi4xMlE4OS44NyAyMi4xMiA4OS4xMCAyMS43N1E4OC4zMiAyMS40MyA4Ny44OSAyMC44M1E4Ny40NiAyMC4yMiA4Ny40NiAxOS40MloiIGZpbGw9IiNGRkZGRkYiLz48cGF0aCBjbGFzcz0ic3ZnX190ZXh0IiBkPSJNMTIyLjQ0IDIyTDEyMC4yNCAyMkwxMjAuMjQgMTMuNjBMMTIyLjE5IDEzLjYwTDEyNS4xNSAxOC40NUwxMjguMDMgMTMuNjBMMTI5Ljk4IDEzLjYwTDEzMC4wMSAyMkwxMjcuODMgMjJMMTI3LjgwIDE3LjU1TDEyNS42NCAyMS4xN0wxMjQuNTkgMjEuMTdMMTIyLjQ0IDE3LjY3TDEyMi40NCAyMlpNMTM2LjU5IDIyTDEzNC4xNiAyMkwxMzcuODcgMTMuNjBMMTQwLjIxIDEzLjYwTDE0My45MyAyMkwxNDEuNDYgMjJMMTQwLjgwIDIwLjM3TDEzNy4yNSAyMC4zN0wxMzYuNTkgMjJaTTEzOS4wMiAxNS45M0wxMzcuOTQgMTguNjFMMTQwLjEwIDE4LjYxTDEzOS4wMiAxNS45M1pNMTUwLjQ2IDIyTDE0OC4wOCAyMkwxNDguMDggMTMuNjBMMTUxLjkzIDEzLjYwUTE1My4wNyAxMy42MCAxNTMuOTEgMTMuOThRMTU0Ljc0IDE0LjM1IDE1NS4yMCAxNS4wNlExNTUuNjYgMTUuNzYgMTU1LjY2IDE2LjcxTDE1NS42NiAxNi43MVExNTUuNjYgMTcuNjIgMTU1LjIzIDE4LjMwUTE1NC44MCAxOC45OCAxNTQuMDEgMTkuMzZMMTU0LjAxIDE5LjM2TDE1NS44MiAyMkwxNTMuMjggMjJMMTUxLjc2IDE5Ljc3TDE1MC40NiAxOS43N0wxNTAuNDYgMjJaTTE1MC40NiAxNS40N0wxNTAuNDYgMTcuOTNMMTUxLjc4IDE3LjkzUTE1Mi41MSAxNy45MyAxNTIuODggMTcuNjFRMTUzLjI2IDE3LjI5IDE1My4yNiAxNi43MUwxNTMuMjYgMTYuNzFRMTUzLjI2IDE2LjEyIDE1Mi44OCAxNS43OVExNTIuNTEgMTUuNDcgMTUxLjc4IDE1LjQ3TDE1MS43OCAxNS40N0wxNTAuNDYgMTUuNDdaTTE2Mi44MCAyMkwxNjAuNDQgMjJMMTYwLjQ0IDEzLjYwTDE2Mi44MCAxMy42MEwxNjIuODAgMTcuMDlMMTY2LjA1IDEzLjYwTDE2OC42NyAxMy42MEwxNjUuMjQgMTcuMzJMMTY4Ljg1IDIyTDE2Ni4wOSAyMkwxNjMuNjkgMTguOTVMMTYyLjgwIDE5LjkwTDE2Mi44MCAyMlpNMTc2LjkzIDIyTDE3Mi45NSAyMkwxNzIuOTUgMTMuNjBMMTc2LjkzIDEzLjYwUTE3OC4zMSAxMy42MCAxNzkuMzggMTQuMTJRMTgwLjQ0IDE0LjYzIDE4MS4wMyAxNS41OFExODEuNjIgMTYuNTMgMTgxLjYyIDE3LjgwTDE4MS42MiAxNy44MFExODEuNjIgMTkuMDcgMTgxLjAzIDIwLjAyUTE4MC40NCAyMC45NyAxNzkuMzggMjEuNDhRMTc4LjMxIDIyIDE3Ni45MyAyMkwxNzYuOTMgMjJaTTE3NS4zMyAxNS41MEwxNzUuMzMgMjAuMTBMMTc2LjgzIDIwLjEwUTE3Ny45MSAyMC4xMCAxNzguNTcgMTkuNDlRMTc5LjIyIDE4Ljg4IDE3OS4yMiAxNy44MEwxNzkuMjIgMTcuODBRMTc5LjIyIDE2LjcyIDE3OC41NyAxNi4xMVExNzcuOTEgMTUuNTAgMTc2LjgzIDE1LjUwTDE3Ni44MyAxNS41MEwxNzUuMzMgMTUuNTBaTTE4NS45MiAxNy44MEwxODUuOTIgMTcuODBRMTg1LjkyIDE2LjU1IDE4Ni41MyAxNS41NVExODcuMTMgMTQuNTYgMTg4LjE5IDE0LjAwUTE4OS4yNiAxMy40MyAxOTAuNTkgMTMuNDNMMTkwLjU5IDEzLjQzUTE5MS45MiAxMy40MyAxOTIuOTggMTQuMDBRMTk0LjA0IDE0LjU2IDE5NC42NSAxNS41NVExOTUuMjYgMTYuNTUgMTk1LjI2IDE3LjgwTDE5NS4yNiAxNy44MFExOTUuMjYgMTkuMDUgMTk0LjY1IDIwLjA0UTE5NC4wNCAyMS4wNCAxOTIuOTggMjEuNjBRMTkxLjkyIDIyLjE3IDE5MC41OSAyMi4xN0wxOTAuNTkgMjIuMTdRMTg5LjI2IDIyLjE3IDE4OC4xOSAyMS42MFExODcuMTMgMjEuMDQgMTg2LjUzIDIwLjA0UTE4NS45MiAxOS4wNSAxODUuOTIgMTcuODBaTTE4OC4zMiAxNy44MEwxODguMzIgMTcuODBRMTg4LjMyIDE4LjUxIDE4OC42MiAxOS4wNVExODguOTIgMTkuNjAgMTg5LjQ0IDE5LjkwUTE4OS45NSAyMC4yMCAxOTAuNTkgMjAuMjBMMTkwLjU5IDIwLjIwUTE5MS4yMiAyMC4yMCAxOTEuNzQgMTkuOTBRMTkyLjI2IDE5LjYwIDE5Mi41NSAxOS4wNVExOTIuODUgMTguNTEgMTkyLjg1IDE3LjgwTDE5Mi44NSAxNy44MFExOTIuODUgMTcuMDkgMTkyLjU1IDE2LjU0UTE5Mi4yNiAxNiAxOTEuNzQgMTUuNzBRMTkxLjIyIDE1LjQwIDE5MC41OSAxNS40MEwxOTAuNTkgMTUuNDBRMTg5Ljk1IDE1LjQwIDE4OS40MyAxNS43MFExODguOTIgMTYgMTg4LjYyIDE2LjU0UTE4OC4zMiAxNy4wOSAxODguMzIgMTcuODBaTTIwMi4wNiAyMkwxOTkuMzQgMTMuNjBMMjAxLjc5IDEzLjYwTDIwMy40OCAxOC45NkwyMDUuMjUgMTMuNjBMMjA3LjQ0IDEzLjYwTDIwOS4xMyAxOS4wMUwyMTAuODkgMTMuNjBMMjEzLjE2IDEzLjYwTDIxMC40NCAyMkwyMDcuODkgMjJMMjA2LjI5IDE2Ljg5TDIwNC42MSAyMkwyMDIuMDYgMjJaTTIyMC4wMSAyMkwyMTcuNjcgMjJMMjE3LjY3IDEzLjYwTDIxOS42MyAxMy42MEwyMjMuMzQgMTguMDdMMjIzLjM0IDEzLjYwTDIyNS42NyAxMy42MEwyMjUuNjcgMjJMMjIzLjcxIDIyTDIyMC4wMSAxNy41MkwyMjAuMDEgMjJaIiBmaWxsPSIjRkZGRkZGIiB4PSIxMTkuMDUiLz48L3N2Zz4=)](https://forthebadge.com)

# Message Components

- Text
- Buttons
- Images
- Markdown
- Bot Typing Indicator

# Usage

You can follow the instructions [here](docs/instructions.md)