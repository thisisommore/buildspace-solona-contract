FROM gitpod/workspace-full
USER gitpod
RUN sh -c "$(curl -sSfL https://release.solana.com/v1.10.32/install)"
ENV PATH="/home/gitpod/.local/share/solana/install/active_release/bin:$PATH"
RUN solana config set --url localhost
RUN npm install -g mocha
RUN cargo install --git https://github.com/project-serum/anchor anchor-cli --locked