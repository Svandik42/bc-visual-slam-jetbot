# Autonomní vizuální SLAM a navigace mobilního robota JetBot

Tento repozitář obsahuje zdrojové kódy a dokumentaci k bakalářské práci zaměřené na návrh a implementaci autonomní navigace kolového robota **Waveshare JetBot** s využitím frameworku **ROS 2**.

## Cíle projektu
Hlavním cílem práce je zprovoznit na platformě NVIDIA Jetson Nano spolehlivý systém pro mapování neznámého prostředí pomocí vizuálního SLAMu a následnou autonomní navigaci robota. Celý systém je zastřešen webovým uživatelským rozhraním.

### Dílčí úkoly:
* Zprovoznění a konfigurace **ROS 2** na mikropočítači Jetson Nano.
* Implementace V-SLAM algoritmu (RTAB-Map / ORB-SLAM3) za použití monokulární kamery (160° FOV).
* Generování a průběžná aktualizace 2D mřížky obsazenosti (Occupancy Grid).
* Nastavení navigačního stacku **Nav2** (konfigurace cenových map, globální a lokální plánovač).
* Tvorba responzivního **webového rozhraní** umožňujícího:
  * Zobrazení živé mapy a telemetrie robota.
  * Odeslání cílové polohy kliknutím do mapy.
  * Přenos obrazu z kamery robota s nastavitelnou kompresí.

## Použité technologie
* **Hardware:** NVIDIA Jetson Nano, Waveshare JetBot, Sony IMX219 (8MP, 160° FOV)
* **Software:** Ubuntu, ROS 2 (Humble/Iron)
* **Klíčové ROS 2 balíčky:** `nav2`, `rtabmap_ros`, `rosbridge_suite`

## Aktuální stav projektu
 V současné době probíhá teoretická rešerše SLAM algoritmů, architektury ROS 2 a příprava vývojového prostředí.
