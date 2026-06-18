.. cmake-manual-description: CMake BitLocker TPM Unlocker Command Line Reference

cmake-bitlocker(7)
==================

NAME
----

cmake-bitlocker - CMake BitLocker Encryption Storage Integration Manual

DESCRIPTION
-----------

The ``--bitlocker-unlock`` capability allows non-interactive drive 
decryption routines to be initiated straight from an unprivileged user space 
shell interface. It interacts directly with the system's local Trusted 
Platform Module (TPM 2.0) stack to securely resolve keys.

COMMAND LINE OPTIONS
--------------------

.. option:: --bitlocker-unlock <device> <mount>

  Initialize the storage extraction loop. Requires the explicit target block 
  device node string path and a local empty folder target directory mount point.

.. option:: --strategy=<auto|sealed|nv>

  Configure the extraction fallback lookup routing priority:

  ``auto``
    Attempts to read structural target PCR-bound key blobs first, falling back 
    to a fixed Non-Volatile (NV) memory registry query layout if unsealing fails.

  ``sealed``
    Forces verification directly against a target system state policy profile 
    (typically PCR 0, 1, 7 for Secure Boot verification).

  ``nv``
    Forces a direct read lookup constraint targeting a raw index address.

.. option:: --blob=<path>

  Specify the concrete system disk string path targeting the encrypted, 
  wrapped TPM binary secret file (Only evaluated under ``sealed`` or ``auto`` strategies).

.. option:: --index=<hex>

  Override the target hexadecimal memory registry register target destination. 
  Defaults explicitly to ``0x1500001`` if omitted.
.. cmake-manual-description: CMake BitLocker TPM Unlocker Command Line Reference

cmake-bitlocker(7)
==================

NAME
----

cmake-bitlocker - CMake BitLocker Encryption Storage Integration Manual

DESCRIPTION
-----------

The ``--bitlocker-unlock`` capability allows non-interactive drive 
decryption routines to be initiated straight from an unprivileged user space 
shell interface. It interacts directly with the system's local Trusted 
Platform Module (TPM 2.0) stack to securely resolve keys.

COMMAND LINE OPTIONS
--------------------

.. option:: --bitlocker-unlock <device> <mount>

  Initialize the storage extraction loop. Requires the explicit target block 
  device node string path and a local empty folder target directory mount point.

.. option:: --strategy=<auto|sealed|nv>

  Configure the extraction fallback lookup routing priority:

  ``auto``
    Attempts to read structural target PCR-bound key blobs first, falling back 
    to a fixed Non-Volatile (NV) memory registry query layout if unsealing fails.

  ``sealed``
    Forces verification directly against a target system state policy profile 
    (typically PCR 0, 1, 7 for Secure Boot verification).

  ``nv``
    Forces a direct read lookup constraint targeting a raw index address.

.. option:: --blob=<path>

  Specify the concrete system disk string path targeting the encrypted, 
  wrapped TPM binary secret file (Only evaluated under ``sealed`` or ``auto`` strategies).

.. option:: --index=<hex>

  Override the target hexadecimal memory registry register target destination. 
  Defaults explicitly to ``0x1500001`` if omitted.
.. cmake-manual-description: CMake BitLocker TPM Unlocker Command Line Reference

cmake-bitlocker(7)
==================

NAME
----

cmake-bitlocker - CMake BitLocker Encryption Storage Integration Manual

DESCRIPTION
-----------

The ``--bitlocker-unlock`` capability allows non-interactive drive 
decryption routines to be initiated straight from an unprivileged user space 
shell interface. It interacts directly with the system's local Trusted 
Platform Module (TPM 2.0) stack to securely resolve keys.

COMMAND LINE OPTIONS
--------------------

.. option:: --bitlocker-unlock <device> <mount>

  Initialize the storage extraction loop. Requires the explicit target block 
  device node string path and a local empty folder target directory mount point.

.. option:: --strategy=<auto|sealed|nv>

  Configure the extraction fallback lookup routing priority:

  ``auto``
    Attempts to read structural target PCR-bound key blobs first, falling back 
    to a fixed Non-Volatile (NV) memory registry query layout if unsealing fails.

  ``sealed``
    Forces verification directly against a target system state policy profile 
    (typically PCR 0, 1, 7 for Secure Boot verification).

  ``nv``
    Forces a direct read lookup constraint targeting a raw index address.

.. option:: --blob=<path>

  Specify the concrete system disk string path targeting the encrypted, 
  wrapped TPM binary secret file (Only evaluated under ``sealed`` or ``auto`` strategies).

.. option:: --index=<hex>

  Override the target hexadecimal memory registry register target destination. 
  Defaults explicitly to ``0x1500001`` if omitted.
