- rebase --onto
  - master -> feature01 を分岐し commit をつむ
  - feature01 -> feature02 を分岐し commit をつむ
  - feature02 を分岐したあとに feature01 に commit をつみ、squash merge する
  - feature02 の最初の commit の親が abcdefg の場合 `$ git rebase —onto master abcdefg feature02` で rebase できる
