FROM golang:latest

# ワークディレクトリ作成
WORKDIR /app

# ホストOSの/apps内全てをWORKDIRにコピー
COPY . ./

# ビルド
RUN go build -o ./server-run ./server

# コンテナの9090ポートを公開
EXPOSE 9090

CMD [ "./server-run" ]
