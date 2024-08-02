ALL_OS = {
    "Linux", "FreeBSD", "Windows XP", "Windows 7", "Windows 10", 
    "Symbian", "Palm OS", "Cisco IOS", "Mac OS", "OpenBSD", 
    "NetBSD", "Solaris", "Android", "iOS", "Windows Vista", 
    "Windows 8", "Windows 8.1", "Ubuntu", "Debian", "Fedora",
    "Kali Linux", "CentOS", "Arch Linux", "Red Hat Enterprise Linux (RHEL)",
    "Mint", "Elementary OS"
}

OS_DB = {
    "DF": {
        True: {
            "FreeBSD", "Linux", "Windows XP", "Windows 7", "Windows 10", 
            "Mac OS", "OpenBSD", "NetBSD", "Solaris", "Windows Vista", 
            "Windows 8", "Windows 8.1", "Ubuntu", "Debian", "Fedora", 
            "Kali Linux", "CentOS", "Arch Linux", "Red Hat Enterprise Linux (RHEL)", 
            "Mint", "Elementary OS"
        },
        False: {
            "FreeBSD", "Symbian", "Palm OS", "Linux", "Windows XP", 
            "Windows 7", "Windows 10", "Cisco IOS", "Android", "iOS"
        }
    },
    "TTL": {
        64: {
            "Linux", "FreeBSD", "Mac OS", "OpenBSD", "NetBSD", "Ubuntu", 
            "Debian", "Fedora", "Kali Linux", "CentOS", "Arch Linux", 
            "Red Hat Enterprise Linux (RHEL)", "Mint", "Elementary OS"
        },
        128: {
            "Windows XP", "Windows 7", "Windows 10", "Windows Vista", 
            "Windows 8", "Windows 8.1", "Android", "iOS"
        },
        255: {"Cisco IOS"},
        256: {"Symbian", "Palm OS"}
    },
    "Win Size": {
        8192: {"Symbian", "Windows 7", "Fedora", "Windows Vista", "Windows 8", "Windows 8.1"},
        14600: {"Linux"},
        16348: {"Palm OS"},
        64240: {"Linux"},
        65392: {"Windows 10"},
        65535: {
            "FreeBSD", "Windows XP", "Windows 10", "Mac OS", "OpenBSD", 
            "NetBSD", "Kali Linux", "CentOS", "Arch Linux", "Red Hat Enterprise Linux (RHEL)"
        },
        65550: {"FreeBSD"},
        5840: {"Linux", "Ubuntu", "Debian"},
        5720: {"Cisco IOS"},
        1460: {"Linux", "Ubuntu", "Debian"},
        65536: {"Solaris"},
        29200: {"Mint", "Elementary OS"},
        None: ALL_OS
    },
    "MSS": {
        1350: {"Palm OS"},
        1440: {"Windows XP", "Windows 7", "Windows 10"},
        1460: {
            "Linux", "FreeBSD", "Windows XP", "Windows 7", "Windows 10", 
            "Symbian", "Mac OS", "Ubuntu", "Debian", "Fedora", "Kali Linux", 
            "CentOS", "Arch Linux", "Red Hat Enterprise Linux (RHEL)", 
            "Mint", "Elementary OS"
        },
        1480: {"Cisco IOS", "Solaris"},
        1380: {"Linux", "Android"},
        1300: {"iOS"}
    },
    "SYN": {
        "WSS=8192": {
            "Linux", "FreeBSD", "Windows XP", "Windows 7", "Windows 10", 
            "Ubuntu", "Debian", "Fedora", "Kali Linux", "CentOS", "Arch Linux", 
            "Red Hat Enterprise Linux (RHEL)", "Mint", "Elementary OS"
        },
        "WSS=14600": {"Linux"},
        "WSS=16348": {"Palm OS"},
        "WSS=65535": {
            "FreeBSD", "Windows XP", "Windows 10", "Mac OS", "OpenBSD", 
            "NetBSD", "Kali Linux", "CentOS", "Arch Linux", "Red Hat Enterprise Linux (RHEL)"
        },
        "WSS=1460": {"Linux", "Ubuntu", "Debian"},
        "WSS=65536": {"Solaris"},
        None: ALL_OS
    },
    "Opcodes": {
        "MSS,NOP,WS,TS,NOP,NOP,SACK": {
            "Linux", "FreeBSD", "Ubuntu", "Debian", "Fedora", "Kali Linux", 
            "CentOS", "Arch Linux", "Red Hat Enterprise Linux (RHEL)", 
            "Mint", "Elementary OS"
        },
        "MSS,WS,TS,NOP,NOP,SACK": {"Windows XP", "Windows 7", "Windows 10", "Mac OS", "Solaris"},
        "MSS,NOP,WS,TS,SACK": {
            "Linux", "FreeBSD", "Windows XP", "Windows 7", "Windows 10", 
            "Ubuntu", "Debian", "Fedora", "Kali Linux", "CentOS", "Arch Linux", 
            "Red Hat Enterprise Linux (RHEL)", "Mint", "Elementary OS"
        },
        "MSS,NOP,WS,TS": {"Symbian", "Palm OS"},
        "MSS,WS,TS,SACK": {"Cisco IOS", "Android"},
        "MSS,NOP,WS,TS,NOP": {"iOS"},
        None: ALL_OS
    },
    "ECN": {
        True: {
            "Linux", "FreeBSD", "Windows 10", "Ubuntu", "Debian", "Fedora", 
            "Kali Linux", "CentOS", "Arch Linux", "Red Hat Enterprise Linux (RHEL)", 
            "Mint", "Elementary OS"
        },
        False: {
            "Windows XP", "Windows 7", "Mac OS", "Symbian", "Palm OS", "Cisco IOS", 
            "Android", "iOS", "Windows Vista", "Windows 8", "Windows 8.1"
        },
        None: ALL_OS
    }
}
