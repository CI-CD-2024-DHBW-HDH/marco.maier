# Klausur 2023 DHBW HDH

## Aufgabe 5

5. Erkläre in eigenen Worten:
   * Welche Vorteile ein Kubernetes Deployment gegenüber einem Kubernetes Pod hat **(2 Punkte)**
   Ein Deployment verwaltet und skaliert automatisch die Anzahl an Pods, je nach Auslastung. Auch kann durch ein Deployment ein Update oder Rollback sehr leicht über alle Pods ausgerollt werden. Weiterhin ist ein Deployment in der Lage automatisch fehlerhafte Pods zu ersetzen um so die Availability zu erhöhen.
   * Wofür ein Kubernetes Service gut ist **(2 Punkte)**
   Ein Kubernetes Service bietet einen DNS-Namen und eine konstante IP-Adresse, über welche man die Pods erreichen kann. Da die Pods dynamisch erstellt und gelöscht werden können, ändern diese sonst ihre Adressen. Außerdem ermöglicht ein Service ein Load-Balancing auf den Pods.
   * Mehrere Wege wie man eine Kubernetes Anwendung von außen erreichen kann **(3 Punkte)**
   Ein NodePort stellt eine Anwendung auf einem Port für alle Nodes des Clusters bereit.
   Läuft die Anwendung bspw. über eine Cloud so kann ein Loadbalancer verwendet werden, um die verschiedenen Pods zu erreichen.
   Ingress ermöglicht es HTTP-Verkehr auf einzelne Services weiterzuleiten.
