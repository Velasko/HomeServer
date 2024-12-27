Storage:
    - Use external disk for data
    - Backup to cloud
        - Only selected content
            - Borg
            - Jellyfin config
        - Automatically download on reinstall
    - Longhorn + zfs ?
        zfs within host + longhorn for container access n' network
    - Ensure no data is erased on reconfiguration

Networking:
    VPN: Netmaker (Wireguard)
        - Declarative & easy user management
        - Isolate subnet access per user
    Firewall: ?
    
Secrets:
    - How to store them
        - Encrypted on GH ?
        - Bitwarden ?
    - Talosconfig structure
        Must separate into multiple files so the secrets can be stored separately.
        So the config is stored on GH w/o worry about leak.
            - How to gen new keys to be used on those

More:
    - Adding more hosts
        - local
            - Use pc as node when powered
            - rpi/new machine
        - Remotely
            - baremetal
            - cloud
        - Have a private decentralized VPN for cluster conection
    - Secure boot
    - gvisor - Container security/isolation
