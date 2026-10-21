================
Changelog-To-Doc
================

This repository collects the TYPO3 Core changelog entries that the official
TYPO3 documentation still has to take over. It holds issues only, no code.

Where the issues come from
==========================

Every merged TYPO3 Core commit that adds, changes, or deletes a file in
``typo3/sysext/core/Documentation/Changelog/`` opens an issue here. The
account ``TYPO3IncTeam`` opens it. A later change to the same changelog file
opens a new issue.

The issue title is the summary of the Core commit. The issue shows the
commit message, the full text of each added changelog file, and the diff of
each changed one.

The issue gets a version label automatically for each folder of a changed
changelog file, such as ``15.0`` or ``14.3.x``. For an added file, the
folder is the earliest version that contains the change. A changed file
keeps the folder of its original entry.

Triage
======

The Documentation Team decides for each issue whether a manual needs a
change, as
`Triage new issues <https://docs.typo3.org/permalink/h2document:changelog-triage>`_
describes:

*   A manual label, such as ``TYPO3 Explained`` or ``TCA reference``, names
    the manual to change. An issue stays open until every labeled manual is
    done.
*   A label ``EXT:<extension>`` names the manual of a system extension.
    These manuals are part of the TYPO3 Core and change through Gerrit, so
    such an issue also gets the label ``Gerrit``: it needs an issue on
    Forge and a change in Gerrit.
*   ``No docs needed`` closes an issue that needs no change, with a comment
    that says why.
*   An issue whose change is already documented is closed with a comment
    that says where, without the label ``No docs needed``.

Work on an issue
================

Read
`Apply Changelog entries to the docs <https://docs.typo3.org/permalink/h2document:howto-update-docs>`_
before you start. It explains how to find the TYPO3 versions that the
change belongs to and which version directive to use. Document each issue
in its own pull request, and put ``Resolves: <issue URL>`` in the commit
message.

To avoid duplicate work, comment on the issue before you start, and check
that nobody else is assigned.

If you use an AI assistant, give it the skills of the guide "How to
document". See
`Skills for TYPO3 documentation <https://docs.typo3.org/permalink/h2document:ai-assistance-skills>`_.
