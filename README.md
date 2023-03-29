# Layers archtecture

![layers](https://user-images.githubusercontent.com/50691459/228539843-143b5d70-33f5-4e2a-aa0c-36eda53251bd.jpg)

 - **Transport:** верхний слой, входящая точка в код, представлен в виде controller-a, command-ы или consumer-а/handler-а. Отвечает за приняетие данных и делегирование их соответствующим сервисам на обработку. 
 - **Domain:** сервисный/доменный слой, уровень бизнес логики. Исключено любое взаимодействие с фреймворками, деталями реализации хранилища и сторонними библиотеками. Любое взаимодействие осуществляется по средствам портов/интерфейсов.
 - **Repository/Gateway:** слой доступа и хранения данных. Логгирование, сетевые взаимодействия, сохраненеие состояния и т.п.
