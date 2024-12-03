# olllama-local
docker compose for local ollama usage


Инструкция по установке gpu 
https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html#installation

Запустить докер
docker run -d --gpus=all -v ollama:/root/.ollama -p 11434:11434 --name ollama ollama/ollama

Запуск 
docker exec -it ollama ollama run llama3.1
docker exec -it ollama ollama run qwen2.5-coder:7b
docker exec -it ollama  ollama run qwen2.5-coder:14b