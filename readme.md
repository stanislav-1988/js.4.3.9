{
	"info": {
		"_postman_id": "ea0c7e51-b28b-4163-a95f-46eb805ed4f8",
		"name": "js core 4.3.9",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json",
		"_exporter_id": "23865563"
	},
	"item": [
		{
			"name": "registr",
			"request": {
				"method": "POST",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n  \"user\": {\r\n    \"username\": \"huligan\",\r\n    \"email\": \"dokwuhctac@gmail.com\",\r\n    \"password\": \"qwerty123\"\r\n  }\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://blog.kata.academy/api/users",
					"protocol": "https",
					"host": [
						"blog",
						"kata",
						"academy"
					],
					"path": [
						"api",
						"users"
					]
				}
			},
			"response": []
		},
		{
			"name": "Login",
			"request": {
				"method": "POST",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n  \"user\": {\r\n    \"email\": \"dokwuhctac@gmail.com\",\r\n    \"password\": \"qwerty123\"\r\n  }\r\n}",
					"options": {
						"raw": {
							"language": "json"
						}
					}
				},
				"url": {
					"raw": "https://blog.kata.academy/api/users/login",
					"protocol": "https",
					"host": [
						"blog",
						"kata",
						"academy"
					],
					"path": [
						"api",
						"users",
						"login"
					]
				}
			},
			"response": []
		},
		{
			"name": "data user",
			"protocolProfileBehavior": {
				"disableBodyPruning": true
			},
			"request": {
				"auth": {
					"type": "oauth2",
					"oauth2": [
						{
							"key": "addTokenTo",
							"value": "header",
							"type": "string"
						}
					]
				},
				"method": "GET",
				"header": [],
				"body": {
					"mode": "raw",
					"raw": "{\r\n  \"user\": {\r\n    \"email\": \"dokwuhctac@gmail.com\",\r\n    \"password\": \"qwerty123\",\r\n    \"username\": \"stanislav\",\r\n    \"bio\": \"frontend-develeper\",\r\n    \"image\": \"sss\"\r\n  }\r\n}"
				},
				"url": {
					"raw": "https://blog.kata.academy/api/user",
					"protocol": "https",
					"host": [
						"blog",
						"kata",
						"academy"
					],
					"path": [
						"api",
						"user"
					]
				}
			},
			"response": []
		}
	]
}
