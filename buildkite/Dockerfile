FROM buildkite/agent
ENV KUSTOMIZE_VER 3.9.1

RUN curl -L https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize%2Fv${KUSTOMIZE_VER}/kustomize_v${KUSTOMIZE_VER}_linux_amd64.tar.gz -o /kustomize.tar.gz \
    && curl -L https://codeclimate.com/downloads/test-reporter/test-reporter-latest-linux-amd64 -o /usr/bin/cc-test-reporter \
    && tar -zxvf /kustomize.tar.gz \
    && mv /kustomize /usr/bin/kustomize \
    && chmod +x /usr/bin/kustomize \
    && chmod +x /usr/bin/cc-test-reporter \
    && git config --global user.email "alves.wm@gmail.com" \
    && git config --global user.name "R. A. Souza"
