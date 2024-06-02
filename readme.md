# Rocket Chat Ansible Project

Dit is een Ansible-project dat tot doel heeft een chattoepassing te maken met behulp van Rocket Chat.

## Vereisten

- Ansible geïnstalleerd op de beheermachine.
- SSH-toegang tot de doelmachine met behulp van SSH-keys.

## Installatie

1. Clone de repository:

   ```bash
   git clone https://github.com/Yentheee/rocket_chat.git
   ```
2. Pas het hosts-bestand aan:

   Open het `hosts`-bestand en wijzig het IP-adres naar het juiste IP-adres van de doelmachine.
3. Voer het Ansible-playbook uit:

   ```bash
   ansible-playbook -i hosts playbook.yml
   ```

## Gebruik

1. Open je webbrowser en ga naar `http://"ip doelmachine":3000`.
2. Meld je aan of log in om de chattoepassing te gebruiken.
3. Maak of sluit je aan bij chatrooms om te beginnen met berichten sturen naar andere gebruikers.

## Semaphore-integratie

Als je Semaphore wilt gebruiken voor CI/CD, moet je eerst het `hosts`-bestand aanpassen zoals hierboven beschreven. Of je pat de inventory in Semaphore aan naar het juiste ip. Vervolgens kun je Semaphore configureren om het Ansible-playbook uit te voeren als onderdeel van je CI/CD-pijplijn.
