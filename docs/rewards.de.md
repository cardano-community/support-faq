  
  
Nachfolgend findest du eine Liste von häufig gestellten Fragen aus Kanälen der Cardano-Community. Wenn du etwas siehst, das nicht beantwortet wurde, melde die Frage bitte über das Symbol in der oberen rechten Ecke :smile:

#### Ich habe in Epoche `n` an einen Pool delegiert, wann erhalte ich meine Belohnungen? {: id="reward-schedule"}
Bei jeder Änderung der Delegation werden die Belohnungen nach 3 Epochenübergängen (also nach `15-20 Tagen`) berücksichtigt. Schau dir die Details unten an, wie es funktioniert:
- Eine Epoche in Cardano ist 5 Tage lang. Jede Änderung in der Delegation wird am Ende der Epoche (beim 1. Epochenübergang) in einem Snapshot festgehalten.
- Der erfasste Snapshot wird beim nächsten (2.) Epochenübergang als *live* betrachtet. Das bedeutet, dass der Pool, an den du delegiert hast, deine Delegation in `n+2` Epochen widerspiegeln würde, um sich für die Chance zu qualifizieren, Blöcke proportional zu seinem Einsatz zu machen (der nun deine Delegation beinhalten würde).
- Die vom Pool erzeugten Blöcke qualifizieren sich für Belohnungen, die beim nächsten Epochenübergang berechnet werden (die Berechnung erfolgt also bei `n+3`).
- Schließlich werden die Rewards dann am Ende der nächsten Epoche `n+3` ausgezahlt.
Wenn du also in Epoche `n` delegiert hast, sind deine Rewards zu Beginn von Epoche `n+4` bei dir (technisch gesehen am Ende von Epoche `n+3`).
Die visuelle Darstellung der obigen Erklärung ist wie unten (mit `n=213` im Beispiel):

  ![Rewards Schedule](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/rewards-schedule.jpg)

#### Verpassen wir Belohnungen, wir an einen anderen Pool delegieren? {: id="change-delegation"}
Nein.
Wenn du innerhalb einer Epoche zweimal zu einem anderen Pool wechselst, wird nur die letzte Änderung beim Epochen-Snapshot erfasst.
Wenn du die Delegation von Pool `P1` zu `P2` änderst, erhälst du weiterhin Belohnungen von Pool `P1`, bis [Reward-Zeitplan](#reward-schedule) für `P2` beginnt.

#### Wie kann ich meine Belohnungen überwachen? Yoroi oder Daedalus zeigt keine epochenweise Verteilung der Belohnungen an {: id="monitor-rewards"}
Yoroi zeigt die Belohnungshistorie an, die jetzt auch als Teil des Exports in CSV verfügbar ist. Für den Fall, dass du nicht in der Lage bist, die Belohnungshistorie in diesm Format zu verwenden, gibt es mehrere Möglichkeiten, deine Belohnungen zu überwachen. Du kannst eine beliebige deiner Wallet-Adressen verwenden (es spielt keine Rolle, welche, wähle eine zufällige Adresse aus deinem Wallet > Registerkarte "Empfangen") um die Belohnungshistorie mit einer der unten genannten Möglichkeiten zu verfolgen:
- via Browser in [pooltool] oder [cardanoscan]
- Benachrichtigungen auf deinem Smartphone erhalten via [PoolTool Mobile App](https://pegasuspool.info/) 
- Telegram-Benachrichtigungen via [ADAstat](https://t.me/AdaStatBot)

#### Ich habe meine Belohnungen nicht erhalten, obwohl ich gemäß dem Zeitplan abgewartet habe. Worauf muss ich achten? {: id="missing-rewards"}
Erste Anlaufstelle ist idealerweise dein Poolbetreiber. Die meisten Poolbetreiber stellen dir eine Möglichkeit zur Verfügung, sie zu kontaktieren. Aber ein paar Hinweise, um die Ursache selbst zu überprüfen:
- Wenn du in Epoche x Belohnungen erwartest, überprüfe die von Pool in x-2 gemachten Blöcke (siehe Zeitplan [oben](#reward-schedule) für Details). Du kannst einen der [Pool Explorer](explorers.md#list) verwenden und mit der Pool-Historie prüfen, ob Blöcke in der letzten Epoche produziert wurden.
- Wenn der Pool zwar Blöcke gemacht hat, du aber keine Belohnungen erhalten hast, überprüfe die Pool-Parameter - wenn die Fixkostengebühr (Standard-Minimum ist 340 ADA) für den Pool höher ist als die Belohnungen, die er ausgibt, kann es sein, dass ein Delegator keine Belohnungen erhält.
- Wenn der Betreiber selbst keine Rewards erhalten hat, kann das auf ein Problem mit seiner Pool-Einrichtung hinweisen, am besten benachrichtigst du ihn so früh wie möglich.

#### Muss ich Belohnungen abheben und erneut delegieren?
Die Belohnungen, die du verdienst, werden automatisch als Teil deiner Delegation dem Pool angerechnet. Dies gilt auch für alle neuen Gelder, auf die du einzahlst oder von der Wallet abhebst. Derzeit ist deine Wallet selbst an einen Pool delegiert, alle Änderungen, die in Epoche `n` auftreten, werden daher automatisch als Teil des Snapshots erfasst und führen zu aktualisierten Rewards in Epoche `n+4`. **Das einzige Mal, dass du deine Belohnungen abheben musst, ist, wenn du dein gesamtes Guthaben in eine andere Wallet/Börse verschiebst. 

[pooltool]: https://pooltool.io
[cardanoscan]: https://cardanoscan.io
[adapools]: https://adapools.org
