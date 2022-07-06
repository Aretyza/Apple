# Apple

При вводе команды /apple, если у игрока есть 50 опыта, выдается n-количество яблок всем игрокам на сервере. Вся настройка в конфиге

API:

1. PlayerGiveAppleEvent ($event) - событие, вызываемое при выполнении команды /apple
1.1 $event->getPlayer() -> обьект игрока, выдавшего яблоки
1.2 $event->getCount() -> количество яблок
1.3 $event->getPlayers() -> массив игроков, получивших яблоки
1.4 $event->setPlayers(array $players) -> устанавливает игроков, которые получат яблоки.

2. TimeoutManager ($timeout_manager)
2.1 Получить - Apple::getInstance()->getTimeoutManager();
2.2 $player - обьект класса pocketmine/player/Player|pocketmine/Player
2.2 $timeout_manager->hasTimeOut($player); // true|false (проверяет есть ли у игрока таймаут)
2.3 $timeout_manager->getTimeOut($player)
// в будущем продолжу
