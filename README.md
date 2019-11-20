# React Rust Webapp

        cargo new --bin react_rust_webapp
        cd react_rust_webapp

        mkdir ui
        cd ui
        npm init -y
        npm install --save react react-dom
        npm install --save-dev babel-core babel-loader babel-preset-env babel-preset-react webpack webpack-cli

        mkdir dist
        touch dist/index.html
        mkdir src
        touch src/index.js

        touch .babelrc

        touch webpack.config.js

        npm i -g webpack-cli

## Test Frontend

        npx webpack --mode development

or
        npx webpack --mode production

## Backend
        ./cargo run

## Call

        http://localhost:5000/


## Target

Result is in ./target

        rustup target add x86_64-unknown-linux-musl

        // see https://www.andrew-thorburn.com/cross-compiling-a-simple-rust-web-app/
        brew install filosottile/musl-cross/musl-cross

        cargo run --target=x86_64-unknown-linux-musl


        cargo build --release --target=x86_64-unknown-linux-musl
