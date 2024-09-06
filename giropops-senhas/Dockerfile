FROM cgr.dev/chainguard/python:latest-dev AS builder
WORKDIR /app
COPY . .
RUN pip install --user --no-cache-dir -r requirements.txt  

FROM cgr.dev/chainguard/python:latest
WORKDIR /app
COPY --from=builder /home/nonroot/.local/lib/python3.12/site-packages /home/nonroot/.local/lib/python3.12/site-packages
COPY --from=builder /home/nonroot/.local/bin/flask /home/nonroot/.local/bin/flask
COPY . .

ENV PATH="/home/nonroot/.local/bin:$PATH"
ENTRYPOINT ["flask", "run", "--host=0.0.0.0"]
