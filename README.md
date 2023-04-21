### Задание 1

- BaaS - это облачный сервис резервного копирования. Основная задача которого заключается в воссстоновлении данных при полной их утрате.
- DRaaS - это виртуальная копия операционной системы, которая позволяет быстро восстановить инфраструктуру посредством высокой скорости восстановления.
- Active-Active - это кластер состоящий как минимум из двух узлов, основная задача которого балансировка нагрузки, чтобы предотвратить перегрузку любого отдельного узла.
- Active-Passive -это тоже кластер, только с той разницей, что пассивный сервер находиться в режиме ожидания и включается в тот момент, когда активный сервер отключен    или имеется большая нагрузка на основной(активный).

---

### Задание 2

Если это для одного сервера, то я бы воспользовался собственным сервером для резервного копирования, хоть он и дороже по сравнению с BaaS(облачный сервис)

Для этой задачи выбор пал на Differential Backup. Хорошее сочетание в котором:
- нагрузка на сеть 
- скорость восстановления данных
- объем пезервных копий
Для этого, самое безболезненое будет создание резервных копий 
- в рабочие дни после 20.00, а лучше ночью делать Differential Backup
- начиная с субботы можно делать полный бэкап, но тоже лучше в ночное время.

---
