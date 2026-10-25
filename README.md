# FarmHud (Enhanced)

An enhanced fork of [FarmHud](https://www.curseforge.com/wow/addons/farmhud) by Hizuro and CodeRedLin. All credit for the original addon goes to the upstream authors; this fork adds a few quality-of-life features on top.

## What changed

- **Route lines clipped to the radar circle.** [Routes](https://www.curseforge.com/wow/addons/routes)' minimap route line (reparented into FarmHud's own radar via `Routes:ReparentMinimap`) used to draw straight past the radar's visible edge. Added a shared circular mask texture, sized/positioned to match the radar's own border graphic, applied to every line (and arrow, see below) segment texture as it appears.
- **Survives Alt+Z.** FarmHud is now parented to `WorldFrame` instead of `UIParent` — Alt+Z works by hiding `UIParent`, so anything parented to it (the old default) disappears along with the rest of the interface. A compensating scale factor keeps the on-screen size identical to before.
- **Automount on loot.** New option (off by default): while the radar is shown and you're not already mounted, looting an item summons a random collected, usable mount marked as Favorite in the Mount Journal (`C_MountJournal`).
- The route-clip mask now also covers [Routes](https://www.curseforge.com/wow/addons/routes)' new optional direction-arrow overlay (see the Routes enhanced fork), not just the plain line.

## Installation

Drop this folder into `Interface/AddOns/FarmHud`. The new option lives in FarmHud's existing config panel, under the general Options group.

---

# FarmHud (улучшенная версия)

Улучшенный форк [FarmHud](https://www.curseforge.com/wow/addons/farmhud) авторства Hizuro и CodeRedLin. Вся заслуга за оригинальный аддон принадлежит авторам; этот форк добавляет несколько улучшений поверх.

## Что изменено

- **Линия маршрута обрезается кругом радара.** Линия маршрута из [Routes](https://www.curseforge.com/wow/addons/routes) (привязанная к радару FarmHud через `Routes:ReparentMinimap`) раньше рисовалась прямо за видимый край радара. Добавлена общая круглая маска-текстура, по размеру и позиции совпадающая с декоративной рамкой радара, применяемая к каждому сегменту линии (и стрелки, см. ниже) по мере их появления.
- **Переживает Alt+Z.** FarmHud теперь привязан к `WorldFrame` вместо `UIParent` — Alt+Z работает именно через скрытие `UIParent`, поэтому всё, что привязано к нему (как было раньше), исчезает вместе с остальным интерфейсом. Компенсирующий масштаб сохраняет визуальный размер таким же, как раньше.
- **Автопризыв маунта при луте.** Новая опция (по умолчанию выключена): пока радар открыт и персонаж ещё не верхом, лут предмета призывает случайный собранный, пригодный к использованию маунт, отмеченный избранным в коллекции (`C_MountJournal`).
- Маска обрезки линии маршрута теперь покрывает и новый необязательный оверлей со стрелками направления из [Routes](https://www.curseforge.com/wow/addons/routes) (см. улучшенный форк Routes), а не только обычную линию.

## Установка

Поместите эту папку в `Interface/AddOns/FarmHud`. Новая опция находится в существующей панели настроек FarmHud, в общей группе Options.
