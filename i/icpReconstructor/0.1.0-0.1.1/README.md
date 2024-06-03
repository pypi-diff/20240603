# Comparing `tmp/icpReconstructor-0.1.0.tar.gz` & `tmp/icpReconstructor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icpReconstructor-0.1.0.tar", last modified: Fri May 10 12:13:01 2024, max compression
+gzip compressed data, was "icpReconstructor-0.1.1.tar", last modified: Mon Jun  3 07:28:31 2024, max compression
```

## Comparing `icpReconstructor-0.1.0.tar` & `icpReconstructor-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 12:13:01.927032 icpReconstructor-0.1.0/
--rw-rw-rw-   0        0        0    35823 2024-05-03 12:19:46.000000 icpReconstructor-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1259 2024-05-10 12:13:01.927032 icpReconstructor-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-05-10 12:04:06.000000 icpReconstructor-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 12:13:01.892583 icpReconstructor-0.1.0/icpReconstructor/
--rw-rw-rw-   0        0        0      590 2024-05-10 12:04:06.000000 icpReconstructor-0.1.0/icpReconstructor/__init__.py
--rw-rw-rw-   0        0        0    37927 2024-05-10 12:04:06.000000 icpReconstructor-0.1.0/icpReconstructor/casadi_reconstruction.py
--rw-rw-rw-   0        0        0    27666 2024-05-10 12:04:06.000000 icpReconstructor-0.1.0/icpReconstructor/epipolar_reconstruction.py
--rw-rw-rw-   0        0        0    39600 2024-05-10 12:04:06.000000 icpReconstructor-0.1.0/icpReconstructor/torch_reconstruction.py
--rw-rw-rw-   0        0        0    32838 2024-05-10 12:04:06.000000 icpReconstructor-0.1.0/icpReconstructor/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:13:01.927032 icpReconstructor-0.1.0/icpReconstructor.egg-info/
--rw-rw-rw-   0        0        0     1259 2024-05-10 12:13:01.000000 icpReconstructor-0.1.0/icpReconstructor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2024-05-10 12:13:01.000000 icpReconstructor-0.1.0/icpReconstructor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 12:13:01.000000 icpReconstructor-0.1.0/icpReconstructor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-05-10 12:13:01.000000 icpReconstructor-0.1.0/icpReconstructor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-10 12:13:01.000000 icpReconstructor-0.1.0/icpReconstructor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-10 12:13:01.927032 icpReconstructor-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1462 2024-05-10 12:09:02.000000 icpReconstructor-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:28:31.049845 icpReconstructor-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-03 07:28:28.000000 icpReconstructor-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-06-03 07:28:31.049845 icpReconstructor-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-06-03 07:28:28.000000 icpReconstructor-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:28:31.049845 icpReconstructor-0.1.1/icpReconstructor/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-03 07:28:28.000000 icpReconstructor-0.1.1/icpReconstructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37060 2024-06-03 07:28:28.000000 icpReconstructor-0.1.1/icpReconstructor/casadi_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27063 2024-06-03 07:28:28.000000 icpReconstructor-0.1.1/icpReconstructor/epipolar_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38761 2024-06-03 07:28:28.000000 icpReconstructor-0.1.1/icpReconstructor/torch_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32129 2024-06-03 07:28:28.000000 icpReconstructor-0.1.1/icpReconstructor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 07:28:31.049845 icpReconstructor-0.1.1/icpReconstructor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-06-03 07:28:31.000000 icpReconstructor-0.1.1/icpReconstructor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-03 07:28:31.000000 icpReconstructor-0.1.1/icpReconstructor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 07:28:31.000000 icpReconstructor-0.1.1/icpReconstructor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-03 07:28:31.000000 icpReconstructor-0.1.1/icpReconstructor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-03 07:28:31.000000 icpReconstructor-0.1.1/icpReconstructor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-03 07:28:31.049845 icpReconstructor-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-06-03 07:28:30.000000 icpReconstructor-0.1.1/setup.py
```

### Comparing `icpReconstructor-0.1.0/LICENSE` & `icpReconstructor-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `icpReconstructor-0.1.0/icpReconstructor/__init__.py` & `icpReconstructor-0.1.1/icpReconstructor/__init__.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,3 +1,3 @@
-from icpReconstructor.torch_reconstruction import TorchParameterizedFunction, Polynomial3Torch, PolynomialKTorch, TorchPolynomialCurve, TorchMovingFrame, TorchCurveEstimator
-from icpReconstructor.casadi_reconstruction import CasadiParameterizedFunction, Polynomial3Casadi, PolynomialKCasadi, CasadiMovingFrame, CasadiCurveEstimator
+from icpReconstructor.torch_reconstruction import TorchParameterizedFunction, Polynomial3Torch, PolynomialKTorch, TorchPolynomialCurve, TorchMovingFrame, TorchCurveEstimator
+from icpReconstructor.casadi_reconstruction import CasadiParameterizedFunction, Polynomial3Casadi, PolynomialKCasadi, CasadiMovingFrame, CasadiCurveEstimator
 from icpReconstructor.utils import fromWorld2Img, image_to_idx, camera_folder_to_params, PixelDataset, ball_tree_norm, brute_force_distance_norm, find_longest_path, discretizeODE, fromWorld2Img, fromWorld2ImgCasadi, spaceCarving, spaceCarvingReconstruction
```

### Comparing `icpReconstructor-0.1.0/icpReconstructor/casadi_reconstruction.py` & `icpReconstructor-0.1.1/icpReconstructor/casadi_reconstruction.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,868 +1,868 @@
-import casadi
-import numpy as np
-from abc import ABC, abstractmethod
-from .utils import discretizeODE, fromWorld2ImgCasadi
-
-
-class CasadiParameterizedFunction(ABC):
-    """
-        Class for storing parameterized functions for usage with Casadi. Allows for fast initialization
-        of corresponding PyTorch modules.
-    """
-
-    @abstractmethod
-    def get_u_fun( self, idx, s0, s1 ):
-        pass
-    
-    @abstractmethod
-    def get_parameters( self ):
-        # Method that outputs the symbolic parameters (decision variables) of the parameterized function.
-        pass
-
-
-class Polynomial3Casadi(CasadiParameterizedFunction):
-    r"""
-       Parameterization of third-order polynomials. The parameters are the function value and the derivative at start and end.
-       This, for example, allows for easy initialization given simulation results from physics-based models.
-
-       .. note::
-           The parameters for the polynomials are given as
-           :math:`up(i,:) = [f(l[i-1]), f'(l[i-1]), f(l[i]), f'(l[i])]`
-
-       Arguments
-       ----------
-       n : int
-           Number of polynomials used to approximate the cr. Typically set to the number of tubes.
-
-       u_p : str or n-by-4 tensor
-           Optional initialization of the curvature parameters.
-
-       continuous : boolean
-           If True, the polynomials are forced to be continuous.
-
-       random_init : boolean
-           If True and u_p is None, the parameters are initialized randomly.
-
-       end_no_curvature : boolean
-           If True, the last polynomial is forced to be 0. This allows for physically more reasonable uz, so
-           :math:`f_n(s) = 0`
-   """
-
-    def __init__( self, opt, n, u_p=None, optimize=True, continuous=False, random_init=False, end_no_curvature=False ):
-        super().__init__()
-        self.n = n
-        self.optimize = optimize
-        if not (u_p is None) and type(u_p) not in [casadi.MX, np.array, np.ndarray]:
-            raise Exception("The provided curvature parameters should either be casadi.MX objects or numpy arrays.")
-        if continuous and optimize:
-            n_f = n - end_no_curvature * 2 + 1
-            n_f_dot = n - end_no_curvature
-            if u_p is None:
-                self.u_params = opt.variable(n_f, 1)
-                self.u_dot_params = opt.variable(n_f_dot, 2)
-                if random_init:
-                    opt.set_initial(self.u_params, 10 * (np.random.randn(n_f, 1) - 0.5))
-                    opt.set_initial(self.u_dot_params, 10 * (np.random.randn(n_f_dot, 2) - 0.5))
-            else:
-                self.u_params = opt.variable(self.n - 1, 1)
-                self.u_dot_params = opt.variable(self.n - 1, 2)
-                opt.set_initial(self.u_params, u_p[:-1, 0, None])
-                opt.set_initial(self.u_dot_params, u_p[:-1, 2:])
-            u_node = casadi.vertcat(self.u_params, casadi.MX.zeros((2, 1))) if end_no_curvature else self.u_params
-            u_dot_node = casadi.vertcat(
-                self.u_dot_params, casadi.MX.zeros((1, 2))
-                ) if end_no_curvature else self.u_dot_params
-            self.u_p = casadi.cse(casadi.horzcat(u_node[:-1, :], u_dot_node[:, 0], u_node[1:, :], u_dot_node[:, 1]))
-        else:
-            if u_p is None and optimize:
-                self.u_p = opt.variable(n, 4)
-                opt.set_initial(self.u_p, 10 * (np.random.rand(n, 4) - 0.5) if random_init else np.zeros((n, 4)))
-            elif u_p is None and not optimize:
-                self.u_p = casadi.MX.zeros((n, 4))
-            elif optimize:
-                self.u_p = opt.variable(n, 4)
-                opt.set_initial(self.u_p, u_p)
-            else:
-                self.u_p = casadi.MX(u_p)
-
-    def get_u_fun( self, idx, s0, s1 ):
-        '''
-            Function for generating the polynomial of degree 3 from the curvature parameters.
-            u = [f(s0), f'(s0), f(s1), f'(s1)]
-        '''
-        u = self.u_p[idx, :]
-        T = s1 - s0
-        a = (2 * u[0] - 2 * u[2] + T * u[1] + T * u[3]) / (T ** 3)
-        b = -(3 * u[0] - 3 * u[2] + 2 * T * u[1] + T * u[3]) / (T ** 2)
-        c = u[1]
-        d = u[0]
-
-        def u_fun( s ):
-            return casadi.horzcat(d, c, b, a) @ ((s - s0) ** (np.arange(0, 4)).reshape(4, 1))
-
-        return u_fun
-
-    def get_value( self, sol ):
-        """
-            Returns the value of the curvature parameters as a PyTorch tensor.
-        """
-        return sol.value(self.u_p)
-    
-    def get_parameters(self):
-        return self.u_p
-
-
-class PolynomialKCasadi(CasadiParameterizedFunction):
-    r"""
-            Parameterization of degree K polynomials. This implementation uses Casadi for the optimization.
-
-            Arguments
-            ----------
-            n : int
-                Number of polynomials used to approximate the cr. Typically set to the number of tubes.
-
-            K : int
-                Degree used for the polynomials.
-
-            u_p : str or n-by-K tensor
-                Optional initialization of the curvature parameters.
-
-            optimize : boolean
-                If True, the parameters are optimized during the fitting process.
-
-            random_init : boolean
-                If True and u_p is None, the parameters are initialized randomly.
-
-            end_no_curvature : boolean
-                If True, the last polynomial is forced to be 0. This allows for physically more reasonable uz, so
-        """
-
-    def __init__( self, opt, n, K, u_p=None, optimize=True, random_init=False, end_no_curvature=False ):
-        super().__init__()
-        self.n = n
-        self.K = K
-        self.optimize = optimize
-        if optimize:
-            n_f = n - end_no_curvature * 2 + 1
-            if u_p is None:
-                self.u_params = opt.variable(n_f, K + 1)
-                opt.set_initial(self.u_params, 10 * (np.random.rand(n_f, K + 1) - 0.5) if random_init else np.zeros((n_f, K + 1)))
-            else:
-                self.u_params = opt.variable(n_f, K + 1)
-                opt.set_initial(self.u_params, u_p[:-1, :])
-            u_node = casadi.vertcat(self.u_params, casadi.MX.zeros((1, K + 1))) if end_no_curvature else self.u_params
-            self.u_p = casadi.horzcat(u_node[:-1, :], u_node[1:, :])
-        else:
-            if u_p is None:
-                self.u_p = casadi.MX.zeros((n, K + 1))
-            else:
-                self.u_p = casadi.MX(u_p)
-
-    def get_u_fun( self, idx, s0, s1 ):
-        '''
-            Function for generating the K-th-ordner polynomial from the curvature parameters.
-        '''
-
-        def u_fun( s ):
-            return self.u_p[idx, :] @ (((s - s0) / (s1 - s0)) ** (np.arange(0, self.K + 1)).reshape(self.K + 1, 1))
-
-        return u_fun
-    
-    def get_parameters(self):
-        return self.u_p
-
-
-class CasadiCurveModel(ABC):
-    r"""
-        Abstract base class for the curve model. This class implements the basic functionality that is needed for all curve models. The curve models
-        themselves are implemented in the subclasses of this class.
-    """
-    
-    def __init__( self ):
-        self.opt = casadi.Opti()
-    
-    @abstractmethod
-    def get_p( self ):
-        # return the symbolic values for the positions along the backbone p
-        pass
-    
-    @abstractmethod
-    def setup( self ):
-        # The setup function is called once at the beginning of the ICP algorithm. It is used for example for setting up the constraints of a problem.
-        pass
-    
-    @abstractmethod
-    def collect_parameters( self ):
-        # Method for requesting from all parameterized functions their corresponding parameters
-        pass
-
-class CasadiMovingFrame(CasadiCurveModel):
-    r"""
-        This class implements the rotation frame formulation for reconstructing a continuum robot's backbone.
-        The parameterization of the curvatures ux, uy, and uz is achieved by providing CasadiParameterizedFunction objects.
-
-        Arguments
-        ----------
-        l : tensor
-            List of the lengths up to which the corresponding polynomial is used. Is
-            typically selected to be each NiTi tube's length outside of the actuation
-            unit.
-
-        p0 : 3-by-1 tensor
-            A 3D point where the CR exits the actuation unit in world
-            coordinates.
-
-        p0_parametric : boolean
-            If True, the initial position p0 is estimated as well.
-
-        R0 : 3-by-3 or 4-by-1 tensor
-            Either a 3-by-3 matrix from SO(3) that describes the orientation of
-            the exiting CR (ref. [1]) or, if R0_parametric is True, tensor of
-            shape (4,). The matrix is then parametrized using quaternions.
-
-        R0_parametric : boolean
-            If True, the initial orientation R0 is estimated as well. To ensure
-            that R0 remains inside SO(3), it is parameterized using quaternions.
-
-        ux : n-by-4 tensor or CasadiParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the x-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        uy : n-by-4 tensor or CasadiParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the y-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        uz : n-by-4 tensor or CasadiParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the z-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        integrator : str
-            Integration method from the following list:
-
-                - "rk1" / "euler"
-                - "rk2" / "midpoint"
-                - "heun"
-                - "rk3" / "simpson"
-                - "rk4"
-                - "3/8"
-
-            The rk4 typically gives a good trade-off between accuracy and speed.
-
-        continuous_u : list of 3 booleans
-            If true, the corresponding curvature [ ux, uy, uz ] is enforced to be continuous.
-
-        random_init : list of 3 booleans
-            If true, the corresponding curvature [ ux, uy, uz ] is randomly initialized.
-
-        Sources
-        ----------
-        [1] 10.1109/TRO.2010.2062570, Rucker, D. Caleb, Bryan A. Jones, and Robert J. Webster III. "A geometrically exact model for externally loaded concentric-tube continuum robots." IEEE transactions on robotics 26.5 (2010): 769-780.
-    """
-
-    
-    def __init__(
-            self, l, p0=np.zeros((3, 1)), p0_parametric=False, R0=np.eye(3, 3), R0_parametric=False, ux=None, uy=None, uz=None,
-            optimize=[True, True, False], n_steps=50, w=0.0, method='rk4', dist_norm=2, continuous_u=[False, False, True], random_init=[False] * 3
-            ):
-        super().__init__()
-        self.opt.solver('ipopt')
-        self.sol = None
-        self.__method = method
-        self.l = l
-        self.n = len(l)
-        self.n_steps = n_steps
-        self.p0 = p0
-        self.continuous_u = continuous_u
-        self.random_init = random_init
-        self.optimize = optimize
-        self.function_parameters = None
-        
-        self.ux_funs = []
-        self.uy_funs = []
-        self.uz_funs = []
-
-        if p0_parametric:
-            self.p0 = self.opt.variable(3, 1)
-        else:
-            self.p0 = p0
-
-        if R0_parametric:
-            # If R0 is parametric, it is assumed to be a quaternion. The quaternion is then normalized and converted to a rotation matrix.
-            q = self.opt.variable(1, 4)
-            self.q = q
-            self.opt.subject_to(casadi.norm_2(q) == 1)
-            # Convert the quaternion to a rotation matrix R0.
-            casadi.MX.zeros((3, 3))
-            self.R0[0, 0] = 1 - 2 * (q[2] ** 2 + q[3] ** 2)
-            self.R0[0, 1] = 2 * (q[1] * q[2] - q[0] * q[3])
-            self.R0[0, 2] = 2 * (q[1] * q[3] + q[0] * q[2])
-            self.R0[1, 0] = 2 * (q[1] * q[2] + q[0] * q[3])
-            self.R0[1, 1] = 1 - 2 * (q[1] ** 2 + q[3] ** 2)
-            self.R0[1, 2] = 2 * (q[2] * q[3] - q[0] * q[1])
-            self.R0[2, 0] = 2 * (q[1] * q[3] - q[0] * q[2])
-            self.R0[2, 1] = 2 * (q[2] * q[3] + q[0] * q[1])
-            self.R0[2, 2] = 1 - 2 * (q[1] ** 2 + q[2] ** 2)
-        else:
-            self.R0 = R0
-
-        self.ux = ux
-        self.uy = uy
-        self.uz = uz
-
-        self.x0 = casadi.vertcat(p0, R0.flatten())
-        self.x_stage = self.opt.variable(12, n_steps - 1)
-        self.x = casadi.horzcat(self.x0, self.x_stage)
-
-        self.s_val = np.linspace(0, self.l[-1], self.n_steps)
-    
-    @property
-    def method( self ):
-        return self.__method
-
-    @method.setter
-    def method( self, value ):
-        if value not in ["rk1", "rk2", "euler", "rk3", "simpson", "heun", "rk4", "3/8"]:
-            raise Exception(
-                f"The given solver method is not valid or available. Please use one of the following solvers: {['rk1', 'rk2', 'euler', 'rk3', 'simpson', 'heun', 'rk4', '3/8']}"
-                )
-        self.__method = value
-
-    @property
-    def ux( self ):
-        return self.__ux
-
-    @ux.setter
-    def ux( self, value ):
-        if issubclass(type(value), CasadiParameterizedFunction):
-            self.__ux = value
-        else:
-            self.__ux = Polynomial3Casadi(
-                self.opt, self.n, value, optimize=self.optimize[0], continuous=self.continuous_u[0], random_init=self.random_init[0]
-                )
-
-    @property
-    def uy( self ):
-        return self.__uy
-
-    @uy.setter
-    def uy( self, value ):
-        if issubclass(type(value), CasadiParameterizedFunction):
-            self.__uy = value
-        else:
-            self.__uy = Polynomial3Casadi(
-                self.opt, self.n, value, optimize=self.optimize[1], continuous=self.continuous_u[1], random_init=self.random_init[1]
-                )
-
-    @property
-    def uz( self ):
-        return self.__uz
-
-    @uz.setter
-    def uz( self, value ):
-        if issubclass(type(value), CasadiParameterizedFunction):
-            self.__uz = value
-        else:
-            self.__uz = Polynomial3Casadi(
-                self.opt, self.n, value, optimize=self.optimize[2], continuous=self.continuous_u[2], random_init=self.random_init[2]
-                )
-
-    def set_funs( self ):
-        """
-        Function that fills the curvature function handles. Unlike the PyTorch implementation, the Casadi implementation does not need to be called every
-        time the curvature parameters are changed. Instead, the curvature functions are set once and then used for the integration.
-        """
-        for u in ["ux", "uy", "uz"]:
-            if not hasattr(self, u):
-                setattr(self, u, None)
-
-        self.s_val = np.linspace(0, self.l[-1], self.n_steps)
-
-        self.ux_funs = [self.ux.get_u_fun(0, 0, self.l[0])]
-        self.uy_funs = [self.uy.get_u_fun(0, 0, self.l[0])]
-        self.uz_funs = [self.uz.get_u_fun(0, 0, self.l[0])]
-
-        for i in range(1, self.n):
-            self.ux_funs.append(self.ux.get_u_fun(i, self.l[i - 1], self.l[i]))
-            self.uy_funs.append(self.uy.get_u_fun(i, self.l[i - 1], self.l[i]))
-            self.uz_funs.append(self.uz.get_u_fun(i, self.l[i - 1], self.l[i]))
-
-    def add_u_constraint( self, ax, lower_bound=None, upper_bound=None ):
-        """
-        Function for adding bounds to the curvature parameters. The constraints are added to the Casadi optimization problem.
-
-        Arguments
-        ----------
-        ax : str
-            The axis for which the curvature parameters are constrained. Can be one of the following: "x", "y", "z".
-
-        lower_bound : double, np.array, or casadi.MX
-            The lower bound for the curvature parameters. If a scalar is given, the same bound is used for all curvature parameters. If instead a vector
-            is given, the bound is set for each curvature parameter individually.
-
-        upper_bound : double, np.array, or casadi.MX
-            The upper bound for the curvature parameters. If a scalar is given, the same bound is used for all curvature parameters. If instead a vector
-            is given, the bound is set for each curvature parameter individually.
-        """
-        if ax == "x":
-            u = self.ux.u_p
-        elif ax == "y":
-            u = self.uy.u_p
-        elif ax == "z":
-            u = self.uz.u_p
-        else:
-            raise Exception(
-                'The given ax is not known, please only provide one of the following axes to constrain: "x", "y", "z".'
-                )
-
-        if lower_bound is not None:
-            if type(lower_bound) is int:
-                self.opt.subject_to(lower_bound <= u[:])
-            else:
-                self.opt.subject_to(lower_bound[:] <= u[:])
-
-        if upper_bound is not None:
-            if type(upper_bound) is int:
-                self.opt.subject_to(u[:] <= upper_bound)
-            else:
-                self.opt.subject_to(u[:] <= upper_bound[:])
-
-    def u_hat( self, s ):
-        """
-            Function for transforming u_p to the necessary skew-symmstric matrix. idx_fun is the index of the curvature function that is active at the current
-            arc-length.
-
-            Arguments
-            ----------
-            s : double
-                The arc-length at which the curvature function is evaluated.
-
-            Returns
-            ----------
-            out_pos : 3-by-3 np.array or casadi.MX
-                The skew-symmetric matrix corresponding to the curvature functions at the arc-length s.
-        """
-        if s <= self.l[-1]:
-            active_tube_idx = np.where(self.l >= s)[0]
-            idx_fun = np.min(active_tube_idx)
-        else:
-            idx_fun = self.n - 1
-        curvature_mat = casadi.MX(np.zeros((3, 3)))
-        ux, uy, uz = self.ux_funs[idx_fun](s), self.uy_funs[idx_fun](s), self.uz_funs[idx_fun](s)
-        curvature_mat[2, 1] = ux
-        curvature_mat[1, 0] = uz
-        curvature_mat[0, 2] = uy
-        return curvature_mat - curvature_mat.T
-
-    def setup( self, s=None ):
-        """
-        Integrates the moving frame formulas using the selected method in the variable self.method and sets the continuity constraints for the
-        full-discretization of the ODE.
-        """
-        
-        for i in range(self.n_steps - 1):
-            # Do normal integration step if no value of s lies between self.s_val[i] and self.s_val[i+1]
-            self.opt.subject_to(
-                casadi.cse(self.x[:, i+1] == discretizeODE(
-                    self.ode, self.method, 12, self.s_val[i+1]-self.s_val[i], self.s_val[i], self.x[:, i]
-                    )
-                )
-            )
-            
-    def integrate( self, s ):
-        """
-        Integrates the moving frame formulas using the selected method in the variable self.method and returns the solution. Is used to reach arc-length steps 
-        between the ones used for the continuity constraints in setup.
-        """
-        x = casadi.MX(12, s.shape[0])
-        for i in range(s.shape[0]):
-            # Find the index j of self.s_val, where self.s_val[j] <= s[i]
-            j = np.where(self.s_val <= s[i])[0][-1]
-            x[:, i] = discretizeODE(
-                self.ode, self.method, 12, s[i]-self.s_val[j], self.s_val[j], self.x[:, j]
-                )
-        return casadi.cse(x)
-
-
-    def ode( self, s, x ):
-        """
-        Right-hand side of the moving frame ODE.
-
-        Arguments
-        ----------
-        s : float
-            The current value of the arc-length.
-
-        x : 12-by-1 casadi.MX
-            The current state x = [p, R]. p is the position of the CR in world coordinates and R is the rotation matrix describing the orientation of the
-            CR at the current arc-length.
-        """
-        R = x[3:].reshape((3, 3))
-
-        dp = R[:, 2]
-        dR = (R @ self.u_hat(s)).reshape((9, 1))
-        return casadi.vertcat(dp, dR)
-    
-    def get_p(self):
-        return self.x[:3,:]
-    
-    def collect_parameters( self ):
-        params = [u.get_parameters()[:] for u in [self.ux, self.uy, self.uz] if u.optimize]
-        self.function_parameters = casadi.vertcat(*params)
-
-class CasadiCurveEstimator:
-    r"""
-        This class implements the Casadi-based curve estimator (CCE) for continuum robots.
-        The CCE takes a parameterized model for the continuum robot - this can be a rotation
-        frame, circular arcs, differentiable rendering model, ... - and optimizes for the
-        torch.parameters using an Iterative Closest Point algorithm.
-
-        Arguments
-        ----------
-        curve_model : nn.Module
-            A 3D point where the CR exits the actuation unit in world
-            coordinates.
-        
-        l : positive scalar
-            List of the lengths up to which the corresponding polynomial is used. Is
-            typically selected to be each NiTi tube's length outside of the actuation
-            unit.
-
-        camera_calibration_parameters : list of dictionaries
-            A list of dictionaries containing the keys
-            "A", "dist", "P", "R", and "T". The function "camera_folder_to_params" can
-            automatically generate this list for you.
-
-        n_steps : int
-            Number of intermediate steps to evaluate the reconstructed CR at.
-            If low, the computation is fast, but for very low values the convergence might
-            be bad. If high, a better solution might be found, at cost of higher computation
-            times.
-
-        w : double
-            Weighting of the two cost functions. 0 (only track distance of pixels to
-            reconstruction) is typically a good value, but if parts of the CR are occluded,
-            increasing w can help.
-
-        dist_norm : int
-            Order of the metric used to penalize distances. Higher values give more cost to big errors.
-    """
-
-    def __init__( self, curve_model, camera_calibration_parameters, l, w=0., n_steps=50, dist_norm=2 ):
-
-        self.camera_calibration_parameters = camera_calibration_parameters
-        self.__bb_pixel_coordinates = None
-        self.curve_model = curve_model
-        self.opt = self.curve_model.opt
-        self.w = w
-
-        self.n_steps = n_steps
-
-        self.dist_norm = dist_norm
-        self.last_integrate_parameters = None
-        self.ode_solution = None
-        
-           
-    def initial_solve( self ):
-        """
-        Do an initial solve of the optimization problem. This is necessary to compute the positions p in the computation of the losses
-        pixel_loss and backbone_loss.
-        """
-        self.curve_model.set_funs()
-        self.curve_model.setup()
-        self.curve_model.collect_parameters()
-        self._set_warmstart_ipopt(1e-15)
-        self.opt.minimize(0)
-        sol = self.opt.solve()
-        self.opt.solver('ipopt')
-        self.sol = sol
-        
-
-    def solve_3d( self, s, pts, lam_2=0 ):
-        """
-        Solve the optimization problem for the given 3D points pts at the estimated positions s. The optimization problem is solved using Casadi. The resulting
-        curvature parameters can then be used to reconstruct the CR's backbone. The program first sets the curvature functions, followed by the construction
-        of the continuity constraints for the Serret-Frenet formulas. The resulting ODE is integrated using the selected method in the variable self.method.
-
-        Arguments
-        ----------
-        s : m-by-1 np.array
-            The arc-lengths at which the 3D points p were estimated.
-
-        pts : m-by-3 np.array
-            The 3D points that were estimated at the arc-lengths s.
-
-        Returns
-        ----------
-        ux : n-by-4 np.array
-            Values of the x-curvature parameters for all x-curvature function.
-
-        uy : n-by-4 np.array
-            Values of the y-curvature parameters for all y-curvature function.
-
-        uz : n-by-4 np.array
-            Values of the z-curvature parameters for all z-curvature function.
-        """
-        self.curve_model.set_funs()
-        self.curve_model.setup()
-        self.curve_model.collect_parameters()
-        x_out = self.curve_model.integrate(s)
-        cost = casadi.sumsqr(x_out[:3,:] - pts)
-        self.opt.minimize(cost+lam_2*(casadi.sumsqr(self.curve_model.function_parameters)))
-        sol = self.opt.solve()
-        self.sol = sol
-
-        ux = self.curve_model.ux.get_value(sol)
-        uy = self.curve_model.uy.get_value(sol)
-        uz = self.curve_model.uz.get_value(sol)
-
-        return ux, uy, uz
-
-    def get_img_coordinates( self ):
-        """
-        Project the computed backbone points to all the images and return the image coordinates.
-        """
-        if self.__bb_pixel_coordinates is None:
-            backbone_pts = self.curve_model.get_p()
-            self.__bb_pixel_coordinates = []
-            for i in range(len(self.camera_calibration_parameters)):
-                self.__bb_pixel_coordinates.append(fromWorld2ImgCasadi(backbone_pts, **self.camera_calibration_parameters[i]).T)
-        return self.__bb_pixel_coordinates
-
-    def get_pixel_diff_idx( self, cr_img_coordinates, img_idx_data ):
-        """
-        Computes for each CR pixel the index of the closest reconstruction pixel.
-
-        Arguments
-        ----------
-        cr_img_coordinates : m-by-2 int
-            Coordinates of CR pixels in image coordinates.
-
-        img_idx_data : m-by-1 int
-            Vector containing the index from which image the corresponding img_coordinates entry was taken.
-        """
-        backbone_img_coordinates = [self.sol.value(i) for i in self.get_img_coordinates()]
-        idx_min_dist = []
-        cr_img_coordinates_sorted = []
-        for i in np.unique(np.unique(img_idx_data)):
-            cr_img_coordinates_i = cr_img_coordinates[img_idx_data == i, :]
-            x_diffs = backbone_img_coordinates[i][:, 0].reshape((-1, 1)) - cr_img_coordinates_i[:, 0].reshape(1, -1)
-            y_diffs = backbone_img_coordinates[i][:, 1].reshape((-1, 1)) - cr_img_coordinates_i[:, 1].reshape(1, -1)
-            distances = (x_diffs ** self.dist_norm + y_diffs ** self.dist_norm) ** (1 / self.dist_norm)
-            idx_min_dist.append(np.argmin(distances, 0))
-            cr_img_coordinates_sorted.append(cr_img_coordinates_i)
-        return idx_min_dist, cr_img_coordinates_sorted
-
-    def pixel_diff( self, cr_img_coordinates, img_idx_data ):
-        """
-        Compute the distance of each CR pixel to the closest reconstruction point in image coordinates using casadi.
-
-        Arguments
-        ----------
-        cr_img_coordinates : m-by-2 int
-            The image coordinates of CR pixels.
-
-        img_idx_data :m-by-1 int
-            The index of the image a point was taken from.
-       """
-        curve_pixel_coordinates = self.get_img_coordinates()
-        diffs = None
-        idx_min_dist, cr_img_coordinates_sorted = self.get_pixel_diff_idx(cr_img_coordinates, img_idx_data)
-        for i in np.unique(img_idx_data):
-            diffs = curve_pixel_coordinates[i][idx_min_dist[i], :] - cr_img_coordinates_sorted[i] if diffs is None else casadi.vertcat(
-                diffs, curve_pixel_coordinates[i][idx_min_dist[i], :] - cr_img_coordinates_sorted[i])
-        return diffs
-
-    def pixel_loss( self, cr_img_coordinates, img_idx_data ):
-        """
-            Computes the average distance of each CR pixel to the corresponding backbone point in casadi.
-        """
-        # Penalizes the minimum distance of each measurement point to the reconstructed curve.
-        diffs = self.pixel_diff(cr_img_coordinates, img_idx_data)
-        return casadi.sum1(casadi.sum2(diffs ** self.dist_norm) ** (1 / self.dist_norm)) / diffs.shape[0]
-
-    def get_backbone_diff_idx( self, cr_img_coordinates, img_idx_data ):
-        """
-        Computes for each backbone point in image coordinates the index of the closest CR pixel .
-
-        Arguments
-        ----------
-        cr_img_coordinates : m-by-2 int
-            Coordinates of CR pixels in image coordinates.
-
-        img_idx_data : m-by-1 int
-            Vector containing the index from which image the corresponding img_coordinates entry was taken.
-        """
-        backbone_img_coordinates = [self.sol.value(i) for i in self.get_img_coordinates()]
-        idx_min_dist = []
-        cr_img_coordinates_sorted = None
-        for i in np.unique(np.unique(img_idx_data)):
-            cr_img_coordinates_i = cr_img_coordinates[img_idx_data == i, :]
-            x_diffs = backbone_img_coordinates[i][:, 0].reshape((-1, 1)) - cr_img_coordinates_i[:, 0].reshape(1, -1)
-            y_diffs = backbone_img_coordinates[i][:, 1].reshape((-1, 1)) - cr_img_coordinates_i[:, 1].reshape(1, -1)
-            distances = (x_diffs ** self.dist_norm + y_diffs ** self.dist_norm) ** (1 / self.dist_norm)
-            idx_min_dist.append(np.argmin(distances, 1))
-            cr_img_coordinates_sorted = [cr_img_coordinates_i] if cr_img_coordinates_sorted is None else cr_img_coordinates_sorted + [
-                cr_img_coordinates_i]
-
-        return idx_min_dist, cr_img_coordinates_sorted
-
-    def backbone_diff( self, cr_img_coordinates, img_idx_data ):
-        """
-        Compute the distance of each CR pixel to the closest reconstruction point in image coordinates.
-
-        Arguments
-        ----------
-        cr_img_coordinates : m-by-2 int
-            The image coordinates of CR pixels.
-
-        img_idx_data :m-by-1 int
-            The index of the image a point was taken from.
-        """
-        curve_pixel_coordinates = self.get_img_coordinates()
-        diffs = None
-        idx_min_dist, cr_img_coordinates_sorted = self.get_backbone_diff_idx(cr_img_coordinates, img_idx_data)
-        for i in np.unique(img_idx_data):
-            diffs = curve_pixel_coordinates[i] - cr_img_coordinates_sorted[i][idx_min_dist[i], :] if diffs is None else casadi.vertcat(
-                diffs, curve_pixel_coordinates[i] - cr_img_coordinates_sorted[i][idx_min_dist[i], :])
-        return diffs
-
-    def backbone_loss( self, cr_img_coordinates, img_idx_data ):
-        """
-            Computes the average distance of each backbone point to the corresponding CR pixel.
-        """
-        # Penalizes the minimum distance of each measurement point to the reconstructed curve.
-        diffs = self.backbone_diff(cr_img_coordinates, img_idx_data)
-        return casadi.sum1(casadi.sum2(diffs ** self.dist_norm) ** (1 / self.dist_norm)) / diffs.shape[0]
-
-    def loss( self, img_coordinates, img_idx_data ):
-        """
-        Combines the two cost as a weighted sum using w as the weight.
-
-        Arguments
-        ----------
-        img_coordinates : m-by-2 np.array
-            Tensor containing the image coordinates of CR pixels.
-
-        img_idx_data :m-by-1 np.array
-            Tensor containing the index of the image a point was taken from.
-       """
-        loss = 0
-        if self.w < 1.:
-            loss += self.pixel_loss(img_coordinates, img_idx_data) * (1 - self.w)
-        if self.w > 0.:
-            loss += self.backbone_loss(img_coordinates, img_idx_data) * self.w
-        return casadi.cse(loss)
-
-    def loss_3d_dist( self, s, pts ):
-        """
-        Computes the sum of the squared distances of the reconstructed 3D points to the estimated 3D points.
-
-        Arguments
-        ----------
-        s : m-by-1 np.array or casadi.MX
-            The arc-lengths at which the 3D points p were estimated.
-
-        pts : m-by-3 np.array or casadi.MX
-            The 3D points that were estimated at the arc-lengths s.
-        """
-        pt_idc_0 = np.argmin(np.abs(self.s_val.reshape(-1, 1) - s.reshape(1, -1)), 0)
-
-        diff = self.x[:3, pt_idc_0] - pts
-        return casadi.sumsqr(diff)
-
-    def reset_bb_pixel_coordinates( self ):
-        """
-            Resets the backbone pixel coordinates to None, so that they are recomputed the next time they are needed. This is useful if the camera parameters
-            change, but typically not necessary. Calling this function may increase computation time as the backbone pixel coordinates are recomputed,
-            instead of reused. This results in a larger computational graph in Casadi than necessary.
-        """
-        self.__bb_pixel_coordinates = None
-    
-    def _warmstart_with_prev(self):
-        """
-        Initializes the optimization variables with values from the previous solution.
-
-        This method is designed to provide a warm start for the optimization process by initializing the current optimization variables with values obtained 
-        from the previous solution. It sets the initial values for both the decision variables (self.opt.x) and the Lagrange multipliers (self.opt.lam_g) based 
-        on the last solution (self.sol). This approach can potentially lead to faster convergence in iterative optimization procedures.
-        """
-        cce_init = [self.sol.value(self.opt.x), self.sol.value(self.opt.lam_g)]
-        self.opt.set_initial(self.opt.x, cce_init[0])
-        self.opt.set_initial(self.opt.lam_g, cce_init[1]) 
-    
-    def icp_step(self, p, img_idx, lam_2=0):
-        """
-        Performs an iterative closest point (ICP) step to align 3D points to a model.
-        
-        This method executes an ICP step using given 3D points, image indices, and an optional regularization parameter. It starts by initializing with previous 
-        state (_warmstart_with_prev). The cost function is computed based on the loss between provided points and model, with an optional L2 regularization term
-        scaled by lam_2. The optimization problem is then solved, and the solution is stored.
-        
-        Arguments
-        ----------
-        p : m-by-3 np.array or casadi.MX
-            The 3D coordinates of points to be aligned. Each row represents a point.
-        
-        img_idx : n-by-1 np.array
-            Indices of the images corresponding to each 3D point.
-        
-        lam_2 : float, optional
-            Regularization parameter for L2 regularization. A higher value increases the weight of regularization in the cost function. Default is 0, indicating no regularization.
-        
-        Returns
-        -------
-        None
-            This method updates the state of the object but does not return any value. The solution to the optimization problem is stored within the object.
-        """
-        self._warmstart_with_prev()
-        loss = self.loss(p, img_idx)
-        if lam_2 > 0:
-            cost = loss + lam_2*(casadi.sumsqr(self.function_parameters))
-        else:
-            cost = loss
-        self.opt.minimize(cost)
-        self.sol = self.opt.solve()
-        return self.sol.value(loss)
-    
-    def _set_warmstart_ipopt(self, val, **kwargs):
-        """
-        Configures the IPOPT solver for warm starting with specified parameters.
-        
-        This method sets up the IPOPT solver with warm start parameters. If additional keyword arguments are provided, they are used to configure the solver. If
-        a list is provided as 'val', the method sets various IPOPT warm start parameters using elements of this list. If 'val' is not a list, it is used for all
-        warm start parameters. This setup can help in achieving faster convergence for the optimization problem by utilizing information from previous solutions.
-        
-        Arguments
-        ----------
-        val : list or float
-            If a list, it should contain values for 'mu_init', 'warm_start_mult_bound_push', 'warm_start_slack_bound_push', 
-            'warm_start_bound_push', 'warm_start_bound_frac', and 'warm_start_slack_bound_frac', in that order. If a float, 
-            the same value is used for all these parameters.
-        
-        **kwargs : dict, optional
-            Additional keyword arguments to pass to the IPOPT solver for customization.
-        
-        Returns
-        -------
-        None
-            This method configures the IPOPT solver within the object but does not return any value.
-        """
-
-        default_params = {
-            'print_level': 0, 
-            'warm_start_init_point': 'yes'
-        }
-    
-        if isinstance(val, list):
-            warmstart_params = ["mu_init", "warm_start_mult_bound_push", "warm_start_slack_bound_push", 
-                                "warm_start_bound_push", "warm_start_bound_frac", "warm_start_slack_bound_frac"]
-            default_params.update({param: value for param, value in zip(warmstart_params, val)})
-        else:
-            default_params.update({param: val for param in ["mu_init", "warm_start_mult_bound_push", 
-                                                            "warm_start_slack_bound_push", "warm_start_bound_push", 
-                                                            "warm_start_bound_frac", "warm_start_slack_bound_frac"]})
-    
+import casadi
+import numpy as np
+from abc import ABC, abstractmethod
+from .utils import discretizeODE, fromWorld2ImgCasadi
+
+
+class CasadiParameterizedFunction(ABC):
+    """
+        Class for storing parameterized functions for usage with Casadi. Allows for fast initialization
+        of corresponding PyTorch modules.
+    """
+
+    @abstractmethod
+    def get_u_fun( self, idx, s0, s1 ):
+        pass
+    
+    @abstractmethod
+    def get_parameters( self ):
+        # Method that outputs the symbolic parameters (decision variables) of the parameterized function.
+        pass
+
+
+class Polynomial3Casadi(CasadiParameterizedFunction):
+    r"""
+       Parameterization of third-order polynomials. The parameters are the function value and the derivative at start and end.
+       This, for example, allows for easy initialization given simulation results from physics-based models.
+
+       .. note::
+           The parameters for the polynomials are given as
+           :math:`up(i,:) = [f(l[i-1]), f'(l[i-1]), f(l[i]), f'(l[i])]`
+
+       Arguments
+       ----------
+       n : int
+           Number of polynomials used to approximate the cr. Typically set to the number of tubes.
+
+       u_p : str or n-by-4 tensor
+           Optional initialization of the curvature parameters.
+
+       continuous : boolean
+           If True, the polynomials are forced to be continuous.
+
+       random_init : boolean
+           If True and u_p is None, the parameters are initialized randomly.
+
+       end_no_curvature : boolean
+           If True, the last polynomial is forced to be 0. This allows for physically more reasonable uz, so
+           :math:`f_n(s) = 0`
+   """
+
+    def __init__( self, opt, n, u_p=None, optimize=True, continuous=False, random_init=False, end_no_curvature=False ):
+        super().__init__()
+        self.n = n
+        self.optimize = optimize
+        if not (u_p is None) and type(u_p) not in [casadi.MX, np.array, np.ndarray]:
+            raise Exception("The provided curvature parameters should either be casadi.MX objects or numpy arrays.")
+        if continuous and optimize:
+            n_f = n - end_no_curvature * 2 + 1
+            n_f_dot = n - end_no_curvature
+            if u_p is None:
+                self.u_params = opt.variable(n_f, 1)
+                self.u_dot_params = opt.variable(n_f_dot, 2)
+                if random_init:
+                    opt.set_initial(self.u_params, 10 * (np.random.randn(n_f, 1) - 0.5))
+                    opt.set_initial(self.u_dot_params, 10 * (np.random.randn(n_f_dot, 2) - 0.5))
+            else:
+                self.u_params = opt.variable(self.n - 1, 1)
+                self.u_dot_params = opt.variable(self.n - 1, 2)
+                opt.set_initial(self.u_params, u_p[:-1, 0, None])
+                opt.set_initial(self.u_dot_params, u_p[:-1, 2:])
+            u_node = casadi.vertcat(self.u_params, casadi.MX.zeros((2, 1))) if end_no_curvature else self.u_params
+            u_dot_node = casadi.vertcat(
+                self.u_dot_params, casadi.MX.zeros((1, 2))
+                ) if end_no_curvature else self.u_dot_params
+            self.u_p = casadi.cse(casadi.horzcat(u_node[:-1, :], u_dot_node[:, 0], u_node[1:, :], u_dot_node[:, 1]))
+        else:
+            if u_p is None and optimize:
+                self.u_p = opt.variable(n, 4)
+                opt.set_initial(self.u_p, 10 * (np.random.rand(n, 4) - 0.5) if random_init else np.zeros((n, 4)))
+            elif u_p is None and not optimize:
+                self.u_p = casadi.MX.zeros((n, 4))
+            elif optimize:
+                self.u_p = opt.variable(n, 4)
+                opt.set_initial(self.u_p, u_p)
+            else:
+                self.u_p = casadi.MX(u_p)
+
+    def get_u_fun( self, idx, s0, s1 ):
+        '''
+            Function for generating the polynomial of degree 3 from the curvature parameters.
+            u = [f(s0), f'(s0), f(s1), f'(s1)]
+        '''
+        u = self.u_p[idx, :]
+        T = s1 - s0
+        a = (2 * u[0] - 2 * u[2] + T * u[1] + T * u[3]) / (T ** 3)
+        b = -(3 * u[0] - 3 * u[2] + 2 * T * u[1] + T * u[3]) / (T ** 2)
+        c = u[1]
+        d = u[0]
+
+        def u_fun( s ):
+            return casadi.horzcat(d, c, b, a) @ ((s - s0) ** (np.arange(0, 4)).reshape(4, 1))
+
+        return u_fun
+
+    def get_value( self, sol ):
+        """
+            Returns the value of the curvature parameters as a PyTorch tensor.
+        """
+        return sol.value(self.u_p)
+    
+    def get_parameters(self):
+        return self.u_p
+
+
+class PolynomialKCasadi(CasadiParameterizedFunction):
+    r"""
+            Parameterization of degree K polynomials. This implementation uses Casadi for the optimization.
+
+            Arguments
+            ----------
+            n : int
+                Number of polynomials used to approximate the cr. Typically set to the number of tubes.
+
+            K : int
+                Degree used for the polynomials.
+
+            u_p : str or n-by-K tensor
+                Optional initialization of the curvature parameters.
+
+            optimize : boolean
+                If True, the parameters are optimized during the fitting process.
+
+            random_init : boolean
+                If True and u_p is None, the parameters are initialized randomly.
+
+            end_no_curvature : boolean
+                If True, the last polynomial is forced to be 0. This allows for physically more reasonable uz, so
+        """
+
+    def __init__( self, opt, n, K, u_p=None, optimize=True, random_init=False, end_no_curvature=False ):
+        super().__init__()
+        self.n = n
+        self.K = K
+        self.optimize = optimize
+        if optimize:
+            n_f = n - end_no_curvature * 2 + 1
+            if u_p is None:
+                self.u_params = opt.variable(n_f, K + 1)
+                opt.set_initial(self.u_params, 10 * (np.random.rand(n_f, K + 1) - 0.5) if random_init else np.zeros((n_f, K + 1)))
+            else:
+                self.u_params = opt.variable(n_f, K + 1)
+                opt.set_initial(self.u_params, u_p[:-1, :])
+            u_node = casadi.vertcat(self.u_params, casadi.MX.zeros((1, K + 1))) if end_no_curvature else self.u_params
+            self.u_p = casadi.horzcat(u_node[:-1, :], u_node[1:, :])
+        else:
+            if u_p is None:
+                self.u_p = casadi.MX.zeros((n, K + 1))
+            else:
+                self.u_p = casadi.MX(u_p)
+
+    def get_u_fun( self, idx, s0, s1 ):
+        '''
+            Function for generating the K-th-ordner polynomial from the curvature parameters.
+        '''
+
+        def u_fun( s ):
+            return self.u_p[idx, :] @ (((s - s0) / (s1 - s0)) ** (np.arange(0, self.K + 1)).reshape(self.K + 1, 1))
+
+        return u_fun
+    
+    def get_parameters(self):
+        return self.u_p
+
+
+class CasadiCurveModel(ABC):
+    r"""
+        Abstract base class for the curve model. This class implements the basic functionality that is needed for all curve models. The curve models
+        themselves are implemented in the subclasses of this class.
+    """
+    
+    def __init__( self ):
+        self.opt = casadi.Opti()
+    
+    @abstractmethod
+    def get_p( self ):
+        # return the symbolic values for the positions along the backbone p
+        pass
+    
+    @abstractmethod
+    def setup( self ):
+        # The setup function is called once at the beginning of the ICP algorithm. It is used for example for setting up the constraints of a problem.
+        pass
+    
+    @abstractmethod
+    def collect_parameters( self ):
+        # Method for requesting from all parameterized functions their corresponding parameters
+        pass
+
+class CasadiMovingFrame(CasadiCurveModel):
+    r"""
+        This class implements the rotation frame formulation for reconstructing a continuum robot's backbone.
+        The parameterization of the curvatures ux, uy, and uz is achieved by providing CasadiParameterizedFunction objects.
+
+        Arguments
+        ----------
+        l : tensor
+            List of the lengths up to which the corresponding polynomial is used. Is
+            typically selected to be each NiTi tube's length outside of the actuation
+            unit.
+
+        p0 : 3-by-1 tensor
+            A 3D point where the CR exits the actuation unit in world
+            coordinates.
+
+        p0_parametric : boolean
+            If True, the initial position p0 is estimated as well.
+
+        R0 : 3-by-3 or 4-by-1 tensor
+            Either a 3-by-3 matrix from SO(3) that describes the orientation of
+            the exiting CR (ref. [1]) or, if R0_parametric is True, tensor of
+            shape (4,). The matrix is then parametrized using quaternions.
+
+        R0_parametric : boolean
+            If True, the initial orientation R0 is estimated as well. To ensure
+            that R0 remains inside SO(3), it is parameterized using quaternions.
+
+        ux : n-by-4 tensor or CasadiParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the x-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        uy : n-by-4 tensor or CasadiParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the y-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        uz : n-by-4 tensor or CasadiParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the z-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        integrator : str
+            Integration method from the following list:
+
+                - "rk1" / "euler"
+                - "rk2" / "midpoint"
+                - "heun"
+                - "rk3" / "simpson"
+                - "rk4"
+                - "3/8"
+
+            The rk4 typically gives a good trade-off between accuracy and speed.
+
+        continuous_u : list of 3 booleans
+            If true, the corresponding curvature [ ux, uy, uz ] is enforced to be continuous.
+
+        random_init : list of 3 booleans
+            If true, the corresponding curvature [ ux, uy, uz ] is randomly initialized.
+
+        Sources
+        ----------
+        [1] 10.1109/TRO.2010.2062570, Rucker, D. Caleb, Bryan A. Jones, and Robert J. Webster III. "A geometrically exact model for externally loaded concentric-tube continuum robots." IEEE transactions on robotics 26.5 (2010): 769-780.
+    """
+
+    
+    def __init__(
+            self, l, p0=np.zeros((3, 1)), p0_parametric=False, R0=np.eye(3, 3), R0_parametric=False, ux=None, uy=None, uz=None,
+            optimize=[True, True, False], n_steps=50, w=0.0, method='rk4', dist_norm=2, continuous_u=[False, False, True], random_init=[False] * 3
+            ):
+        super().__init__()
+        self.opt.solver('ipopt')
+        self.sol = None
+        self.__method = method
+        self.l = l
+        self.n = len(l)
+        self.n_steps = n_steps
+        self.p0 = p0
+        self.continuous_u = continuous_u
+        self.random_init = random_init
+        self.optimize = optimize
+        self.function_parameters = None
+        
+        self.ux_funs = []
+        self.uy_funs = []
+        self.uz_funs = []
+
+        if p0_parametric:
+            self.p0 = self.opt.variable(3, 1)
+        else:
+            self.p0 = p0
+
+        if R0_parametric:
+            # If R0 is parametric, it is assumed to be a quaternion. The quaternion is then normalized and converted to a rotation matrix.
+            q = self.opt.variable(1, 4)
+            self.q = q
+            self.opt.subject_to(casadi.norm_2(q) == 1)
+            # Convert the quaternion to a rotation matrix R0.
+            casadi.MX.zeros((3, 3))
+            self.R0[0, 0] = 1 - 2 * (q[2] ** 2 + q[3] ** 2)
+            self.R0[0, 1] = 2 * (q[1] * q[2] - q[0] * q[3])
+            self.R0[0, 2] = 2 * (q[1] * q[3] + q[0] * q[2])
+            self.R0[1, 0] = 2 * (q[1] * q[2] + q[0] * q[3])
+            self.R0[1, 1] = 1 - 2 * (q[1] ** 2 + q[3] ** 2)
+            self.R0[1, 2] = 2 * (q[2] * q[3] - q[0] * q[1])
+            self.R0[2, 0] = 2 * (q[1] * q[3] - q[0] * q[2])
+            self.R0[2, 1] = 2 * (q[2] * q[3] + q[0] * q[1])
+            self.R0[2, 2] = 1 - 2 * (q[1] ** 2 + q[2] ** 2)
+        else:
+            self.R0 = R0
+
+        self.ux = ux
+        self.uy = uy
+        self.uz = uz
+
+        self.x0 = casadi.vertcat(p0, R0.flatten())
+        self.x_stage = self.opt.variable(12, n_steps - 1)
+        self.x = casadi.horzcat(self.x0, self.x_stage)
+
+        self.s_val = np.linspace(0, self.l[-1], self.n_steps)
+    
+    @property
+    def method( self ):
+        return self.__method
+
+    @method.setter
+    def method( self, value ):
+        if value not in ["rk1", "rk2", "euler", "rk3", "simpson", "heun", "rk4", "3/8"]:
+            raise Exception(
+                f"The given solver method is not valid or available. Please use one of the following solvers: {['rk1', 'rk2', 'euler', 'rk3', 'simpson', 'heun', 'rk4', '3/8']}"
+                )
+        self.__method = value
+
+    @property
+    def ux( self ):
+        return self.__ux
+
+    @ux.setter
+    def ux( self, value ):
+        if issubclass(type(value), CasadiParameterizedFunction):
+            self.__ux = value
+        else:
+            self.__ux = Polynomial3Casadi(
+                self.opt, self.n, value, optimize=self.optimize[0], continuous=self.continuous_u[0], random_init=self.random_init[0]
+                )
+
+    @property
+    def uy( self ):
+        return self.__uy
+
+    @uy.setter
+    def uy( self, value ):
+        if issubclass(type(value), CasadiParameterizedFunction):
+            self.__uy = value
+        else:
+            self.__uy = Polynomial3Casadi(
+                self.opt, self.n, value, optimize=self.optimize[1], continuous=self.continuous_u[1], random_init=self.random_init[1]
+                )
+
+    @property
+    def uz( self ):
+        return self.__uz
+
+    @uz.setter
+    def uz( self, value ):
+        if issubclass(type(value), CasadiParameterizedFunction):
+            self.__uz = value
+        else:
+            self.__uz = Polynomial3Casadi(
+                self.opt, self.n, value, optimize=self.optimize[2], continuous=self.continuous_u[2], random_init=self.random_init[2]
+                )
+
+    def set_funs( self ):
+        """
+        Function that fills the curvature function handles. Unlike the PyTorch implementation, the Casadi implementation does not need to be called every
+        time the curvature parameters are changed. Instead, the curvature functions are set once and then used for the integration.
+        """
+        for u in ["ux", "uy", "uz"]:
+            if not hasattr(self, u):
+                setattr(self, u, None)
+
+        self.s_val = np.linspace(0, self.l[-1], self.n_steps)
+
+        self.ux_funs = [self.ux.get_u_fun(0, 0, self.l[0])]
+        self.uy_funs = [self.uy.get_u_fun(0, 0, self.l[0])]
+        self.uz_funs = [self.uz.get_u_fun(0, 0, self.l[0])]
+
+        for i in range(1, self.n):
+            self.ux_funs.append(self.ux.get_u_fun(i, self.l[i - 1], self.l[i]))
+            self.uy_funs.append(self.uy.get_u_fun(i, self.l[i - 1], self.l[i]))
+            self.uz_funs.append(self.uz.get_u_fun(i, self.l[i - 1], self.l[i]))
+
+    def add_u_constraint( self, ax, lower_bound=None, upper_bound=None ):
+        """
+        Function for adding bounds to the curvature parameters. The constraints are added to the Casadi optimization problem.
+
+        Arguments
+        ----------
+        ax : str
+            The axis for which the curvature parameters are constrained. Can be one of the following: "x", "y", "z".
+
+        lower_bound : double, np.array, or casadi.MX
+            The lower bound for the curvature parameters. If a scalar is given, the same bound is used for all curvature parameters. If instead a vector
+            is given, the bound is set for each curvature parameter individually.
+
+        upper_bound : double, np.array, or casadi.MX
+            The upper bound for the curvature parameters. If a scalar is given, the same bound is used for all curvature parameters. If instead a vector
+            is given, the bound is set for each curvature parameter individually.
+        """
+        if ax == "x":
+            u = self.ux.u_p
+        elif ax == "y":
+            u = self.uy.u_p
+        elif ax == "z":
+            u = self.uz.u_p
+        else:
+            raise Exception(
+                'The given ax is not known, please only provide one of the following axes to constrain: "x", "y", "z".'
+                )
+
+        if lower_bound is not None:
+            if type(lower_bound) is int:
+                self.opt.subject_to(lower_bound <= u[:])
+            else:
+                self.opt.subject_to(lower_bound[:] <= u[:])
+
+        if upper_bound is not None:
+            if type(upper_bound) is int:
+                self.opt.subject_to(u[:] <= upper_bound)
+            else:
+                self.opt.subject_to(u[:] <= upper_bound[:])
+
+    def u_hat( self, s ):
+        """
+            Function for transforming u_p to the necessary skew-symmstric matrix. idx_fun is the index of the curvature function that is active at the current
+            arc-length.
+
+            Arguments
+            ----------
+            s : double
+                The arc-length at which the curvature function is evaluated.
+
+            Returns
+            ----------
+            out_pos : 3-by-3 np.array or casadi.MX
+                The skew-symmetric matrix corresponding to the curvature functions at the arc-length s.
+        """
+        if s <= self.l[-1]:
+            active_tube_idx = np.where(self.l >= s)[0]
+            idx_fun = np.min(active_tube_idx)
+        else:
+            idx_fun = self.n - 1
+        curvature_mat = casadi.MX(np.zeros((3, 3)))
+        ux, uy, uz = self.ux_funs[idx_fun](s), self.uy_funs[idx_fun](s), self.uz_funs[idx_fun](s)
+        curvature_mat[2, 1] = ux
+        curvature_mat[1, 0] = uz
+        curvature_mat[0, 2] = uy
+        return curvature_mat - curvature_mat.T
+
+    def setup( self, s=None ):
+        """
+        Integrates the moving frame formulas using the selected method in the variable self.method and sets the continuity constraints for the
+        full-discretization of the ODE.
+        """
+        
+        for i in range(self.n_steps - 1):
+            # Do normal integration step if no value of s lies between self.s_val[i] and self.s_val[i+1]
+            self.opt.subject_to(
+                casadi.cse(self.x[:, i+1] == discretizeODE(
+                    self.ode, self.method, 12, self.s_val[i+1]-self.s_val[i], self.s_val[i], self.x[:, i]
+                    )
+                )
+            )
+            
+    def integrate( self, s ):
+        """
+        Integrates the moving frame formulas using the selected method in the variable self.method and returns the solution. Is used to reach arc-length steps 
+        between the ones used for the continuity constraints in setup.
+        """
+        x = casadi.MX(12, s.shape[0])
+        for i in range(s.shape[0]):
+            # Find the index j of self.s_val, where self.s_val[j] <= s[i]
+            j = np.where(self.s_val <= s[i])[0][-1]
+            x[:, i] = discretizeODE(
+                self.ode, self.method, 12, s[i]-self.s_val[j], self.s_val[j], self.x[:, j]
+                )
+        return casadi.cse(x)
+
+
+    def ode( self, s, x ):
+        """
+        Right-hand side of the moving frame ODE.
+
+        Arguments
+        ----------
+        s : float
+            The current value of the arc-length.
+
+        x : 12-by-1 casadi.MX
+            The current state x = [p, R]. p is the position of the CR in world coordinates and R is the rotation matrix describing the orientation of the
+            CR at the current arc-length.
+        """
+        R = x[3:].reshape((3, 3))
+
+        dp = R[:, 2]
+        dR = (R @ self.u_hat(s)).reshape((9, 1))
+        return casadi.vertcat(dp, dR)
+    
+    def get_p(self):
+        return self.x[:3,:]
+    
+    def collect_parameters( self ):
+        params = [u.get_parameters()[:] for u in [self.ux, self.uy, self.uz] if u.optimize]
+        self.function_parameters = casadi.vertcat(*params)
+
+class CasadiCurveEstimator:
+    r"""
+        This class implements the Casadi-based curve estimator (CCE) for continuum robots.
+        The CCE takes a parameterized model for the continuum robot - this can be a rotation
+        frame, circular arcs, differentiable rendering model, ... - and optimizes for the
+        torch.parameters using an Iterative Closest Point algorithm.
+
+        Arguments
+        ----------
+        curve_model : nn.Module
+            A 3D point where the CR exits the actuation unit in world
+            coordinates.
+        
+        l : positive scalar
+            List of the lengths up to which the corresponding polynomial is used. Is
+            typically selected to be each NiTi tube's length outside of the actuation
+            unit.
+
+        camera_calibration_parameters : list of dictionaries
+            A list of dictionaries containing the keys
+            "A", "dist", "P", "R", and "T". The function "camera_folder_to_params" can
+            automatically generate this list for you.
+
+        n_steps : int
+            Number of intermediate steps to evaluate the reconstructed CR at.
+            If low, the computation is fast, but for very low values the convergence might
+            be bad. If high, a better solution might be found, at cost of higher computation
+            times.
+
+        w : double
+            Weighting of the two cost functions. 0 (only track distance of pixels to
+            reconstruction) is typically a good value, but if parts of the CR are occluded,
+            increasing w can help.
+
+        dist_norm : int
+            Order of the metric used to penalize distances. Higher values give more cost to big errors.
+    """
+
+    def __init__( self, curve_model, camera_calibration_parameters, l, w=0., n_steps=50, dist_norm=2 ):
+
+        self.camera_calibration_parameters = camera_calibration_parameters
+        self.__bb_pixel_coordinates = None
+        self.curve_model = curve_model
+        self.opt = self.curve_model.opt
+        self.w = w
+
+        self.n_steps = n_steps
+
+        self.dist_norm = dist_norm
+        self.last_integrate_parameters = None
+        self.ode_solution = None
+        
+           
+    def initial_solve( self ):
+        """
+        Do an initial solve of the optimization problem. This is necessary to compute the positions p in the computation of the losses
+        pixel_loss and backbone_loss.
+        """
+        self.curve_model.set_funs()
+        self.curve_model.setup()
+        self.curve_model.collect_parameters()
+        self._set_warmstart_ipopt(1e-15)
+        self.opt.minimize(0)
+        sol = self.opt.solve()
+        self.opt.solver('ipopt')
+        self.sol = sol
+        
+
+    def solve_3d( self, s, pts, lam_2=0 ):
+        """
+        Solve the optimization problem for the given 3D points pts at the estimated positions s. The optimization problem is solved using Casadi. The resulting
+        curvature parameters can then be used to reconstruct the CR's backbone. The program first sets the curvature functions, followed by the construction
+        of the continuity constraints for the Serret-Frenet formulas. The resulting ODE is integrated using the selected method in the variable self.method.
+
+        Arguments
+        ----------
+        s : m-by-1 np.array
+            The arc-lengths at which the 3D points p were estimated.
+
+        pts : m-by-3 np.array
+            The 3D points that were estimated at the arc-lengths s.
+
+        Returns
+        ----------
+        ux : n-by-4 np.array
+            Values of the x-curvature parameters for all x-curvature function.
+
+        uy : n-by-4 np.array
+            Values of the y-curvature parameters for all y-curvature function.
+
+        uz : n-by-4 np.array
+            Values of the z-curvature parameters for all z-curvature function.
+        """
+        self.curve_model.set_funs()
+        self.curve_model.setup()
+        self.curve_model.collect_parameters()
+        x_out = self.curve_model.integrate(s)
+        cost = casadi.sumsqr(x_out[:3,:] - pts)
+        self.opt.minimize(cost+lam_2*(casadi.sumsqr(self.curve_model.function_parameters)))
+        sol = self.opt.solve()
+        self.sol = sol
+
+        ux = self.curve_model.ux.get_value(sol)
+        uy = self.curve_model.uy.get_value(sol)
+        uz = self.curve_model.uz.get_value(sol)
+
+        return ux, uy, uz
+
+    def get_img_coordinates( self ):
+        """
+        Project the computed backbone points to all the images and return the image coordinates.
+        """
+        if self.__bb_pixel_coordinates is None:
+            backbone_pts = self.curve_model.get_p()
+            self.__bb_pixel_coordinates = []
+            for i in range(len(self.camera_calibration_parameters)):
+                self.__bb_pixel_coordinates.append(fromWorld2ImgCasadi(backbone_pts, **self.camera_calibration_parameters[i]).T)
+        return self.__bb_pixel_coordinates
+
+    def get_pixel_diff_idx( self, cr_img_coordinates, img_idx_data ):
+        """
+        Computes for each CR pixel the index of the closest reconstruction pixel.
+
+        Arguments
+        ----------
+        cr_img_coordinates : m-by-2 int
+            Coordinates of CR pixels in image coordinates.
+
+        img_idx_data : m-by-1 int
+            Vector containing the index from which image the corresponding img_coordinates entry was taken.
+        """
+        backbone_img_coordinates = [self.sol.value(i) for i in self.get_img_coordinates()]
+        idx_min_dist = []
+        cr_img_coordinates_sorted = []
+        for i in np.unique(np.unique(img_idx_data)):
+            cr_img_coordinates_i = cr_img_coordinates[img_idx_data == i, :]
+            x_diffs = backbone_img_coordinates[i][:, 0].reshape((-1, 1)) - cr_img_coordinates_i[:, 0].reshape(1, -1)
+            y_diffs = backbone_img_coordinates[i][:, 1].reshape((-1, 1)) - cr_img_coordinates_i[:, 1].reshape(1, -1)
+            distances = (x_diffs ** self.dist_norm + y_diffs ** self.dist_norm) ** (1 / self.dist_norm)
+            idx_min_dist.append(np.argmin(distances, 0))
+            cr_img_coordinates_sorted.append(cr_img_coordinates_i)
+        return idx_min_dist, cr_img_coordinates_sorted
+
+    def pixel_diff( self, cr_img_coordinates, img_idx_data ):
+        """
+        Compute the distance of each CR pixel to the closest reconstruction point in image coordinates using casadi.
+
+        Arguments
+        ----------
+        cr_img_coordinates : m-by-2 int
+            The image coordinates of CR pixels.
+
+        img_idx_data :m-by-1 int
+            The index of the image a point was taken from.
+       """
+        curve_pixel_coordinates = self.get_img_coordinates()
+        diffs = None
+        idx_min_dist, cr_img_coordinates_sorted = self.get_pixel_diff_idx(cr_img_coordinates, img_idx_data)
+        for i in np.unique(img_idx_data):
+            diffs = curve_pixel_coordinates[i][idx_min_dist[i], :] - cr_img_coordinates_sorted[i] if diffs is None else casadi.vertcat(
+                diffs, curve_pixel_coordinates[i][idx_min_dist[i], :] - cr_img_coordinates_sorted[i])
+        return diffs
+
+    def pixel_loss( self, cr_img_coordinates, img_idx_data ):
+        """
+            Computes the average distance of each CR pixel to the corresponding backbone point in casadi.
+        """
+        # Penalizes the minimum distance of each measurement point to the reconstructed curve.
+        diffs = self.pixel_diff(cr_img_coordinates, img_idx_data)
+        return casadi.sum1(casadi.sum2(diffs ** self.dist_norm) ** (1 / self.dist_norm)) / diffs.shape[0]
+
+    def get_backbone_diff_idx( self, cr_img_coordinates, img_idx_data ):
+        """
+        Computes for each backbone point in image coordinates the index of the closest CR pixel .
+
+        Arguments
+        ----------
+        cr_img_coordinates : m-by-2 int
+            Coordinates of CR pixels in image coordinates.
+
+        img_idx_data : m-by-1 int
+            Vector containing the index from which image the corresponding img_coordinates entry was taken.
+        """
+        backbone_img_coordinates = [self.sol.value(i) for i in self.get_img_coordinates()]
+        idx_min_dist = []
+        cr_img_coordinates_sorted = None
+        for i in np.unique(np.unique(img_idx_data)):
+            cr_img_coordinates_i = cr_img_coordinates[img_idx_data == i, :]
+            x_diffs = backbone_img_coordinates[i][:, 0].reshape((-1, 1)) - cr_img_coordinates_i[:, 0].reshape(1, -1)
+            y_diffs = backbone_img_coordinates[i][:, 1].reshape((-1, 1)) - cr_img_coordinates_i[:, 1].reshape(1, -1)
+            distances = (x_diffs ** self.dist_norm + y_diffs ** self.dist_norm) ** (1 / self.dist_norm)
+            idx_min_dist.append(np.argmin(distances, 1))
+            cr_img_coordinates_sorted = [cr_img_coordinates_i] if cr_img_coordinates_sorted is None else cr_img_coordinates_sorted + [
+                cr_img_coordinates_i]
+
+        return idx_min_dist, cr_img_coordinates_sorted
+
+    def backbone_diff( self, cr_img_coordinates, img_idx_data ):
+        """
+        Compute the distance of each CR pixel to the closest reconstruction point in image coordinates.
+
+        Arguments
+        ----------
+        cr_img_coordinates : m-by-2 int
+            The image coordinates of CR pixels.
+
+        img_idx_data :m-by-1 int
+            The index of the image a point was taken from.
+        """
+        curve_pixel_coordinates = self.get_img_coordinates()
+        diffs = None
+        idx_min_dist, cr_img_coordinates_sorted = self.get_backbone_diff_idx(cr_img_coordinates, img_idx_data)
+        for i in np.unique(img_idx_data):
+            diffs = curve_pixel_coordinates[i] - cr_img_coordinates_sorted[i][idx_min_dist[i], :] if diffs is None else casadi.vertcat(
+                diffs, curve_pixel_coordinates[i] - cr_img_coordinates_sorted[i][idx_min_dist[i], :])
+        return diffs
+
+    def backbone_loss( self, cr_img_coordinates, img_idx_data ):
+        """
+            Computes the average distance of each backbone point to the corresponding CR pixel.
+        """
+        # Penalizes the minimum distance of each measurement point to the reconstructed curve.
+        diffs = self.backbone_diff(cr_img_coordinates, img_idx_data)
+        return casadi.sum1(casadi.sum2(diffs ** self.dist_norm) ** (1 / self.dist_norm)) / diffs.shape[0]
+
+    def loss( self, img_coordinates, img_idx_data ):
+        """
+        Combines the two cost as a weighted sum using w as the weight.
+
+        Arguments
+        ----------
+        img_coordinates : m-by-2 np.array
+            Tensor containing the image coordinates of CR pixels.
+
+        img_idx_data :m-by-1 np.array
+            Tensor containing the index of the image a point was taken from.
+       """
+        loss = 0
+        if self.w < 1.:
+            loss += self.pixel_loss(img_coordinates, img_idx_data) * (1 - self.w)
+        if self.w > 0.:
+            loss += self.backbone_loss(img_coordinates, img_idx_data) * self.w
+        return casadi.cse(loss)
+
+    def loss_3d_dist( self, s, pts ):
+        """
+        Computes the sum of the squared distances of the reconstructed 3D points to the estimated 3D points.
+
+        Arguments
+        ----------
+        s : m-by-1 np.array or casadi.MX
+            The arc-lengths at which the 3D points p were estimated.
+
+        pts : m-by-3 np.array or casadi.MX
+            The 3D points that were estimated at the arc-lengths s.
+        """
+        pt_idc_0 = np.argmin(np.abs(self.s_val.reshape(-1, 1) - s.reshape(1, -1)), 0)
+
+        diff = self.x[:3, pt_idc_0] - pts
+        return casadi.sumsqr(diff)
+
+    def reset_bb_pixel_coordinates( self ):
+        """
+            Resets the backbone pixel coordinates to None, so that they are recomputed the next time they are needed. This is useful if the camera parameters
+            change, but typically not necessary. Calling this function may increase computation time as the backbone pixel coordinates are recomputed,
+            instead of reused. This results in a larger computational graph in Casadi than necessary.
+        """
+        self.__bb_pixel_coordinates = None
+    
+    def _warmstart_with_prev(self):
+        """
+        Initializes the optimization variables with values from the previous solution.
+
+        This method is designed to provide a warm start for the optimization process by initializing the current optimization variables with values obtained 
+        from the previous solution. It sets the initial values for both the decision variables (self.opt.x) and the Lagrange multipliers (self.opt.lam_g) based 
+        on the last solution (self.sol). This approach can potentially lead to faster convergence in iterative optimization procedures.
+        """
+        cce_init = [self.sol.value(self.opt.x), self.sol.value(self.opt.lam_g)]
+        self.opt.set_initial(self.opt.x, cce_init[0])
+        self.opt.set_initial(self.opt.lam_g, cce_init[1]) 
+    
+    def icp_step(self, p, img_idx, lam_2=0):
+        """
+        Performs an iterative closest point (ICP) step to align 3D points to a model.
+        
+        This method executes an ICP step using given 3D points, image indices, and an optional regularization parameter. It starts by initializing with previous 
+        state (_warmstart_with_prev). The cost function is computed based on the loss between provided points and model, with an optional L2 regularization term
+        scaled by lam_2. The optimization problem is then solved, and the solution is stored.
+        
+        Arguments
+        ----------
+        p : m-by-3 np.array or casadi.MX
+            The 3D coordinates of points to be aligned. Each row represents a point.
+        
+        img_idx : n-by-1 np.array
+            Indices of the images corresponding to each 3D point.
+        
+        lam_2 : float, optional
+            Regularization parameter for L2 regularization. A higher value increases the weight of regularization in the cost function. Default is 0, indicating no regularization.
+        
+        Returns
+        -------
+        None
+            This method updates the state of the object but does not return any value. The solution to the optimization problem is stored within the object.
+        """
+        self._warmstart_with_prev()
+        loss = self.loss(p, img_idx)
+        if lam_2 > 0:
+            cost = loss + lam_2*(casadi.sumsqr(self.function_parameters))
+        else:
+            cost = loss
+        self.opt.minimize(cost)
+        self.sol = self.opt.solve()
+        return self.sol.value(loss)
+    
+    def _set_warmstart_ipopt(self, val, **kwargs):
+        """
+        Configures the IPOPT solver for warm starting with specified parameters.
+        
+        This method sets up the IPOPT solver with warm start parameters. If additional keyword arguments are provided, they are used to configure the solver. If
+        a list is provided as 'val', the method sets various IPOPT warm start parameters using elements of this list. If 'val' is not a list, it is used for all
+        warm start parameters. This setup can help in achieving faster convergence for the optimization problem by utilizing information from previous solutions.
+        
+        Arguments
+        ----------
+        val : list or float
+            If a list, it should contain values for 'mu_init', 'warm_start_mult_bound_push', 'warm_start_slack_bound_push', 
+            'warm_start_bound_push', 'warm_start_bound_frac', and 'warm_start_slack_bound_frac', in that order. If a float, 
+            the same value is used for all these parameters.
+        
+        **kwargs : dict, optional
+            Additional keyword arguments to pass to the IPOPT solver for customization.
+        
+        Returns
+        -------
+        None
+            This method configures the IPOPT solver within the object but does not return any value.
+        """
+
+        default_params = {
+            'print_level': 0, 
+            'warm_start_init_point': 'yes'
+        }
+    
+        if isinstance(val, list):
+            warmstart_params = ["mu_init", "warm_start_mult_bound_push", "warm_start_slack_bound_push", 
+                                "warm_start_bound_push", "warm_start_bound_frac", "warm_start_slack_bound_frac"]
+            default_params.update({param: value for param, value in zip(warmstart_params, val)})
+        else:
+            default_params.update({param: val for param in ["mu_init", "warm_start_mult_bound_push", 
+                                                            "warm_start_slack_bound_push", "warm_start_bound_push", 
+                                                            "warm_start_bound_frac", "warm_start_slack_bound_frac"]})
+    
         self.opt.solver('ipopt', {}, {**default_params, **kwargs})
```

### Comparing `icpReconstructor-0.1.0/icpReconstructor/epipolar_reconstruction.py` & `icpReconstructor-0.1.1/icpReconstructor/epipolar_reconstruction.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,603 +1,603 @@
-import cv2
-import math
-import numpy as np
-from scipy.io import loadmat
-from matplotlib import pyplot as plt
-from skimage.morphology import skeletonize
-from scipy.spatial.distance import cdist
-from .utils import find_longest_path
-
-#%%
-
-class EpipolarReconstructor:    
-    
-    r"""
-       Reconstruction through Epipolar geometry. 
-
-       Arguments
-       ----------
-       
-       img_0, img_1 : array
-           Photo in cam.0 and Photo in cam.1
-       
-       A0, A1, dist0, dist1, P0, P1, R, T : array
-           camera matrix
-           A0 and A1 are the intrinsic camera matrices for camera 0 and camera 1.
-           dist0 and dist1 represent the radial distortion coefficients.
-           P0 and P1 are the projection matrices for camera 0 and camera 1.
-           R stands for the rotation matrix, and T represents the translation vector.
-           
-       bin_threshold : int
-           Set pixel value greater than or equal to bin_threshold to 255 and less than bin_threshold to 0, The recommended value is 200.
-       
-       tip_estimator_params_0, tip_estimator_params_1 : store data in MATLAB
-           Defines the initial points and initial directions of the skeleton in camera 0 and camera 1.
-
-       Sources
-       ----------
-       Hartley, R., & Zisserman, A. (2004). Epipolar Geometry and the Fundamental Matrix. In Multiple View Geometry in Computer Vision (pp. 239-261). Cambridge: Cambridge University Press. doi:10.1017/CBO9780511811685.014
-    """
-    
-    def __init__(self, img_0, img_1, A0, A1, dist0, dist1, P0, P1, R, T, bin_threshold, tip_estimator_params_0, tip_estimator_params_1):
-        # Initialise variables:
-        self.img_0 = img_0 # Photo in cam.0
-        self.img_1 = img_1 # Photo in cam.1
-        
-        # camera matrix
-        self.A0 = A0 
-        self.A1 = A1 
-        self.dist0 = dist0
-        self.dist1 = dist1
-        self.P0 = P0 
-        self.P1 = P1
-        self.R = R
-        self.T = T
-        
-        self.bin_threshold = bin_threshold
-        
-        self.tip_estimator_params_0 = tip_estimator_params_0
-        self.tip_estimator_params_1 = tip_estimator_params_1
-          
-    def compute_fundamental_matrix(self, K1, K2, R, t):
-        r"""
-           By using fundamental matrix, the epipolar line in one camera can be generated from a point in anather camera. 
-           The fundamental matrix can be calculated from camera matrix using the formula (9.2) in [1]. 
-           
-           Sources
-           ----------
-           [1] Hartley, R., & Zisserman, A. (2004). Epipolar Geometry and the Fundamental Matrix. In Multiple View Geometry in Computer Vision (pp. 239-261). Cambridge: Cambridge University Press. doi:10.1017/CBO9780511811685.014
-
-         """
-        A = np.dot(K1, np.dot(R.T, t)).flatten()
-        C = np.array([[0, -A[2], A[1]], [A[2], 0, -A[0]], [-A[1], A[0], 0]])
-        ret = np.dot(np.linalg.inv(K2).T, np.dot(R, np.dot(K1.T, C)))
-        return ret
-        
-    def get_2D (self, plot = False):
-        
-        r"""
-           Obtain the skeletons of images from camera 1 and camera 2, and arrange the pixel coordinates of the skeletons in the order of the path from the starting point.
-
-           Arguments
-           ----------
-           plot : boolean
-               If True, images in camera 0 and camera 1 are displayed.
-           
-           data_cam_0, data_cam_1 : array in size (n,2), n is the number of pixels in the skeletons of images from camera 0 and camera 1.
-               The first two elements of the return value of the 'get_2D' function.
-               The 2D coordinates of each point in the skeletons of images from camera 0 and camera 1 are arranged in the order of the path from the starting point.           
-           
-           kan_img_open_0, kan_img_open_1 : array
-               The third and fourth elements of the return value of the 'get_2D' function.
-               Images in camera 0 and camera 1
-         """
-         
-        
-        # Pick the desired points for projection
-        # img in cam.0
-        if len(self.img_0.shape) == 3:
-            img = cv2.cvtColor(self.img_0, cv2.COLOR_BGR2GRAY)
-        else:
-            img = self.img_0    
-
-        param_dict = loadmat(self.tip_estimator_params_0)
-        p_start = param_dict["p_start"]
-        exit_dir = param_dict["exit_dir"]
-        
-        # filter noise
-        se = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (5,5))
-        kan_img_open_0 = cv2.morphologyEx(img, cv2.MORPH_OPEN, se)
-
-        kan_img_open_0[kan_img_open_0 >= self.bin_threshold] = 255
-        kan_img_open_0[kan_img_open_0 < self.bin_threshold] = 0
-
-        # invert the image 
-        kan_img_open_0 = 255-kan_img_open_0
-
-        # get skeleton of img0
-        img_skel = np.array(skeletonize(kan_img_open_0/255))*255
-        m,n = np.where(img_skel==255)    
-        skeleton_0 = np.array([n,m]).T
-        
-        # selekt and arrange the pixel coordinates of the skeleton_0
-        sk_0_ordered = find_longest_path(skeleton_0, p_start)
-        
-        # Remove distortion so that the epipolar line will not shift
-        sk_0_ordered = cv2.undistortPoints(sk_0_ordered.astype(np.float32), self.A0, self.dist0, P = self.A0)
-        sk_0_ordered = np.squeeze(sk_0_ordered)
-            
-        if(plot):
-            plt.figure(1)
-            plt.scatter(sk_0_ordered[:,0],sk_0_ordered[:,1])
-            plt.xlim(0, self.img_0.shape[1])
-            plt.ylim(0, self.img_0.shape[0])
-            plt.xlabel('u')
-            plt.ylabel('v')
-            plt.title('skeleton in cam.0')
-            ax = plt.gca() 
-            ax.invert_yaxis()
-               
-        # Positiondata for the skeleton in img0
-        data_cam_0 = sk_0_ordered 
-        
-        # Read img in cam.1 and skeletonize    
-        img_bgr = self.img_1
-        
-        if len(img_bgr.shape) == 3:
-            img = cv2.cvtColor(img_bgr, cv2.COLOR_BGR2GRAY)
-        else:
-            img = img_bgr
-
-        tip_estimator_params = self.tip_estimator_params_1
-        param_dict = loadmat(tip_estimator_params)
-        p_start = param_dict["p_start"]
-        exit_dir = param_dict["exit_dir"]
-        blank_idc = param_dict["blank_idc"]
-        
-        # filter noise
-        se = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (5,5))
-        kan_img_open_1 = cv2.morphologyEx(img, cv2.MORPH_OPEN, se)
-
-        kan_img_open_1[kan_img_open_1 >= self.bin_threshold] = 255
-        kan_img_open_1[kan_img_open_1 < self.bin_threshold] = 0
-
-        # invert the image 
-        kan_img_open_1 = 255-kan_img_open_1
-        
-        # get skeletion of img1
-        img_skel = np.array(skeletonize(kan_img_open_1 /255))*255
-        m,n = np.where(img_skel==255)
-        skeleton_1 = np.array([n,m]).T
-        
-        # selekt and arrange the pixel coordinates of the skeleton_1
-        sk_1_ordered = find_longest_path(skeleton_1, p_start)
-        
-        # Remove distortion, the identification of insertion point of epiplorline should be applied in undistorted image
-        sk_1_ordered = cv2.undistortPoints(sk_1_ordered.astype(np.float32), self.A1, self.dist1, P = self.A1)
-        sk_1_ordered = np.squeeze(sk_1_ordered)
-            
-        if(plot): 
-            plt.figure(2)
-            plt.scatter(sk_1_ordered[:,0],sk_1_ordered[:,1])
-            plt.xlim(0, self.img_1.shape[1])
-            plt.ylim(0, self.img_1.shape[0])
-            plt.xlabel('u')
-            plt.ylabel('v')
-            plt.title('skeleton in cam.1')
-            ax = plt.gca() 
-            ax.invert_yaxis()
-               
-        # Positiondata for the skeleton in img0
-        data_cam_1 = sk_1_ordered 
-        
-        return (data_cam_0, data_cam_1, kan_img_open_0, kan_img_open_1)
-    
-    def get_3D (self, data_cam_0=None, data_cam_1=None, interval = 20, plot=True):
-        
-        r"""
-           Obtain the 3D coordinates of the skeleton based on the 2D coordinates data in camera 0 and camera 1.
-           To establish correspondences for each point in the skeleton from camera 0 and camera 1, the points in the skeleton from camera 0 are projected into camera 1 using the fundamental matrix. 
-           The intersection points between the skeleton in camera 1 and the projection lines are identified as the corresponding points from camera 0.
-           
-           Arguments
-           ---------
-           data_cam_0, data_cam_1 : array in size (n,2), n is the number of pixels in the skeletons of images from camera 0 and camera 1.
-               The 2D coordinates of each point in the skeletons of images from camera 0 and camera 1, which arranged in the order of the path from the starting point.           
-           
-           interval : int
-               Determines how often projection lines are cast from camera 0 in camera 1 to search for corresponding points in camera 2. 
-               Increasing the interval value appropriately can reduce the algorithm's computation time.
-               
-           plot : boolean
-               If True, images in camera 0 and camera 1 as well as the 3D reconstruction, are displayed.
-         """
-        
-        # Extract rotation and translation matrices from projection matrices. Calculate fundamental matrix 
-
-        R_t_0 = np.dot(np.linalg.inv(self.A0),self.P0)
-        R_t_1 = np.dot(np.linalg.inv(self.A1),self.P1)
-
-        R0 = R_t_0[:, :3] 
-        t0 = R_t_0[:, 3] 
-        t0 = t0.reshape(-1, 1) 
-
-        R1 = R_t_1[:, :3] 
-        t1 = R_t_1[:, 3]
-        t1 = t1.reshape(-1, 1) 
-
-        R1_0 = np.dot(R1, R0.T)
-        t1_0 = np.dot(R1, -np.dot(R0.T, t0)) + t1
-
-        F = self.compute_fundamental_matrix(self.A0, self.A1, R1_0, t1_0)
-        F = np.array([[float(F[i][j]) for j in range(3)] for i in range(3)], dtype=np.float32)
-        
-        if data_cam_0.any()==None or data_cam_1.any()==None:
-            data_cam_0, data_cam_1 = self.get_2D (plot)
-            
-        else:
-            if (plot):
-                plt.figure(1)
-                plt.scatter(data_cam_0[:,0],data_cam_0[:,1])
-                plt.xlim(0, self.img_0.shape[1])
-                plt.ylim(0, self.img_0.shape[0])
-                plt.xlabel('u')
-                plt.ylabel('v')
-                plt.title('skeleton in cam.0')
-                ax = plt.gca() 
-                ax.invert_yaxis()
-                
-                plt.figure(2)
-                plt.scatter(data_cam_1[:,0],data_cam_1[:,1])
-                plt.xlim(0, self.img_1.shape[1])
-                plt.ylim(0, self.img_1.shape[0])
-                plt.xlabel('u')
-                plt.ylabel('v')
-                plt.title('skeleton in cam.1')
-                ax = plt.gca() 
-                ax.invert_yaxis()
-                                
-        sk_0_ordered = data_cam_0 [::interval]
-        sk_1_ordered = data_cam_1
-        
-        pos_list = []
-        data_3d_list = []
-
-        for i in range(sk_0_ordered.shape[0]):
-                      
-            points_camera_0 = sk_0_ordered[i]
-            
-            # Calculate epilines in camera 1 corresponding to points in camera A
-            line_B = cv2.computeCorrespondEpilines(points_camera_0[np.newaxis, :], 0, F) 
-            line_B = np.array(line_B).ravel()
-            a, b, c = line_B
-            
-            if (plot):
-                plt.figure(1)
-                plt.scatter(sk_0_ordered[i,0],sk_0_ordered[i,1],color='r')
-                plt.pause(0.1)
-                
-                plt.figure(2)
-                x_line_B = np.arange(0,self.img_1.shape[1],1)
-                y_line_B = -(a * x_line_B  + c) / b
-                plt.plot(x_line_B ,y_line_B,color='r' ,alpha =0.4)
-                plt.pause(0.1)
-                     
-            # Find intersection of epilines in camera 0
-            distances = np.array([abs(a * x + b * y + c) / np.sqrt(a**2 + b**2) for x, y in sk_1_ordered])
-
-            sorted_indices = np.argsort(distances)
-            sorted_skeleton_1 = [sk_1_ordered[i] for i in sorted_indices]
-            
-            distance = cdist(sorted_skeleton_1[0][np.newaxis, :], sorted_skeleton_1[1:10])
-            distance =  np.array(distance).ravel()
-            
-            param_dict = loadmat(self.tip_estimator_params_1)
-            p_start = param_dict["p_start"]
-            
-            if i == 0:
-                point_1_list = []
-                pre_point_1 = p_start
-                
-                for k in range(len(sorted_skeleton_1)):
-                    
-                    if cdist(sorted_skeleton_1[k][np.newaxis, :], pre_point_1) < 100:
-                        points_camera_1 = sorted_skeleton_1[k]                                          
-                        pos_camera = cv2.triangulatePoints(self.P0, self.P1, points_camera_0, points_camera_1)
-                        pos_camera = np.swapaxes(pos_camera, 0, 1)
-                        pos_camera = cv2.convertPointsFromHomogeneous(pos_camera)
-                        pos_camera = np.array(pos_camera).ravel()
-                        
-                        pos = self.R@pos_camera + self.T
-                        
-                        pos_old = [0,0,0]
-                        length = np.linalg.norm(pos - pos_old)
-                        
-                        pos_old = pos
-                        
-                        pre_point_1 = points_camera_1
-                        sorted_indices_pre = sorted_indices[k]
-                        point_1_list.append(list (points_camera_1))
-                        
-                        if (plot):
-                            plt.figure(2)
-                            plt.scatter(points_camera_1[0],points_camera_1[1],c="g")
-                        
-                        break
-            else: 
-                
-                for k in range(len(sorted_skeleton_1)):
-                    
-                    if sorted_indices_pre < 5:
-                        direction_bb = (sk_1_ordered[sorted_indices_pre+5][0]-sk_1_ordered[sorted_indices_pre][0]), (sk_1_ordered[sorted_indices_pre+5][1]-sk_1_ordered[sorted_indices_pre][1])              
-                    elif sk_1_ordered.shape[0] - sorted_indices_pre < 6:
-                        direction_bb = (sk_1_ordered[sorted_indices_pre][0]-sk_1_ordered[sorted_indices_pre-5][0]), (sk_1_ordered[sorted_indices_pre][1]-sk_1_ordered[sorted_indices_pre-5][1])              
-                    else:
-                        direction_bb = (sk_1_ordered[sorted_indices_pre+5][0]-sk_1_ordered[sorted_indices_pre-5][0]), (sk_1_ordered[sorted_indices_pre+5][1]-sk_1_ordered[sorted_indices_pre-5][1])    
-                    
-                    magnitude = math.sqrt(direction_bb[0]**2 + direction_bb[1]**2)
-                    direction_bb_unit = (direction_bb[0]/magnitude, direction_bb[1]/magnitude)
-                    
-                    direction_ziel = (sk_1_ordered[sorted_indices[k]][0]-pre_point_1[0]), (sk_1_ordered[sorted_indices[k]][1]-pre_point_1[1])
-                    magnitude = math.sqrt(direction_ziel[0]**2 + direction_ziel[1]**2)
-                    direction_ziel_unit = (direction_ziel[0]/magnitude, direction_ziel[1]/magnitude)
-                                   
-                    if cdist(sorted_skeleton_1[k][np.newaxis, :], pre_point_1[np.newaxis, :]) < 50 and np.dot(direction_bb_unit, direction_ziel_unit) > 0.8:
-                        points_camera_1 = sorted_skeleton_1[k]
-                        pre_point_1 = points_camera_1
-                        sorted_indices_pre = sorted_indices[k]
-                        point_1_list.append(list (points_camera_1))
-                        
-                        if (plot):
-                            plt.figure(2)                            
-                            plt.scatter(points_camera_1[0],points_camera_1[1],color='r')               
-                            plt.pause(0.1)                   
-                        
-                        pos_camera = cv2.triangulatePoints(self.P0, self.P1, points_camera_0, points_camera_1)
-                        pos_camera = np.swapaxes(pos_camera, 0, 1)
-                        pos_camera = cv2.convertPointsFromHomogeneous(pos_camera)
-                        pos_camera = np.array(pos_camera).ravel()
-                        
-                        pos = self.R@pos_camera + self.T
-                        
-                        length = length + np.linalg.norm(pos - pos_old)
-                        data_3d = np.append(pos,length)  
-                        
-                        pos_list.append(pos)
-                        data_3d_list.append(data_3d)
-                        
-                        pos_old = pos  
-                
-                        break    
-                
-        if(plot):
-            fig = plt.figure(3)
-            ax = fig.add_subplot(111, projection='3d')       
-            pos_list = np.array(pos_list)
-            ax.scatter(pos_list[:, 0], pos_list[:, 1], pos_list[:, 2], c='r', marker='o')
-            ax.set_xlabel('X')        
-            ax.set_ylabel('Y')        
-            ax.set_zlabel('Z')          
-            ax.set_box_aspect([1, 1, 1])
-            
-        return np.stack(data_3d_list, 0 )
-    
-    
-    def get_3D_faster (self, data_cam_0=None, data_cam_1=None, interval = 20, segments = 10, plot=True):
-        
-        r"""
-           Instead of using projection lines to establish correspondences for each point in the skeletons of images from camera 0 and camera 1, 
-           the 'get_3D_faster' method divides 'skeleton_0' and 'skeleton_1' into multiple segments, 
-           ensuring that the points within each segment in camera 0 and camera 1 correspond evenly to each other.
-           
-           Arguments
-           ---------
-           data_cam_0, data_cam_1 : array in size (n,2), n is the number of pixels in the skeletons of images from camera 0 and camera 1.
-               The 2D coordinates of each point in the skeletons of images from camera 0 and camera 1, which arranged in the order of the path from the starting point.           
-           
-           interval : int
-               Determines how often projection lines are cast from camera 0 in camera 1 to search for corresponding points in camera 2. 
-               Increasing the interval value appropriately can reduce the algorithm's computation time.
-           
-           segments : int
-               The number of segments into which the skeleton in camera 0 and camera 1 is divided.
-               
-           plot : boolean
-               If True, images in camera 0 and camera 1 as well as the 3D reconstruction, are displayed.
-         """
-        
-        # Extract rotation and translation matrices from projection matrices. Calculate fundamental matrix 
-
-        R_t_0 = np.dot(np.linalg.inv(self.A0),self.P0)
-        R_t_1 = np.dot(np.linalg.inv(self.A1),self.P1)
-
-        R0 = R_t_0[:, :3] 
-        t0 = R_t_0[:, 3] 
-        t0 = t0.reshape(-1, 1) 
-
-        R1 = R_t_1[:, :3] 
-        t1 = R_t_1[:, 3]
-        t1 = t1.reshape(-1, 1) 
-
-        R1_0 = np.dot(R1, R0.T)
-        t1_0 = np.dot(R1, -np.dot(R0.T, t0)) + t1
-
-        F = self.compute_fundamental_matrix(self.A0, self.A1, R1_0, t1_0)
-        F = np.array([[float(F[i][j]) for j in range(3)] for i in range(3)], dtype=np.float32)
-        
-        if data_cam_0.any()==None or data_cam_1.any()==None:
-            data_cam_0, data_cam_1 = self.get_2D (plot)
-            
-        else:
-            if (plot):
-                plt.figure(1)
-                plt.scatter(data_cam_0[:,0],data_cam_0[:,1])
-                plt.xlim(0, self.img_0.shape[1])
-                plt.ylim(0, self.img_0.shape[0])
-                plt.xlabel('u')
-                plt.ylabel('v')
-                plt.title('skeleton in cam.0')
-                ax = plt.gca() 
-                ax.invert_yaxis()
-                
-                plt.figure(2)
-                plt.scatter(data_cam_1[:,0],data_cam_1[:,1])
-                plt.xlim(0, self.img_1.shape[1])
-                plt.ylim(0, self.img_1.shape[0])
-                plt.xlabel('u')
-                plt.ylabel('v')
-                plt.title('skeleton in cam.1')
-                ax = plt.gca() 
-                ax.invert_yaxis()
-                
-        sk_0_ordered = data_cam_0 [::interval]
-        sk_1_ordered = data_cam_1
-        
-        pos_list = []
-        data_3d_list = []       
-
-        for i in range(sk_0_ordered.shape[0]):
-                     
-            points_camera_0 = sk_0_ordered[i]
-            points_camera_0 = np.array(points_camera_0, dtype = np.float32)
-            points_undist_0 = cv2.undistortPoints(points_camera_0, self.A0, self.dist0, P = self.A0)
-            
-            # Calculate epilines in camera 1 corresponding to points in camera A
-            line_B = cv2.computeCorrespondEpilines(points_undist_0, 0, F) 
-            line_B = np.array(line_B).ravel()
-            a, b, c = line_B
-            
-            if (plot):
-                plt.figure(1)
-                plt.scatter(sk_0_ordered[i,0],sk_0_ordered[i,1],color='r')
-                plt.pause(0.1)
-                
-                plt.figure(2)
-                x_line_B = np.arange(0,self.img_1.shape[1],1)
-                y_line_B = -(a * x_line_B  + c) / b
-                plt.plot(x_line_B ,y_line_B,color='r' ,alpha =0.4)
-                plt.pause(0.1)
-                    
-            # Find intersection of epilines in camera 0
-            distances = np.array([abs(a * x + b * y + c) / np.sqrt(a**2 + b**2) for x, y in sk_1_ordered])
-
-            sorted_indices = np.argsort(distances)
-            sorted_skeleton_1 = [sk_1_ordered[i] for i in sorted_indices]
-            
-            distance = cdist(sorted_skeleton_1[0][np.newaxis, :], sorted_skeleton_1[1:10])
-            distance =  np.array(distance).ravel()
-            
-            # only one crosspoint for one epiline
-            if max (distance) < 20:
-                
-                points_camera_1 = sorted_skeleton_1[0]                      
-                pos_camera = cv2.triangulatePoints(self.P0, self.P1, points_camera_0, points_camera_1)
-                pos_camera = np.swapaxes(pos_camera, 0, 1)
-                pos_camera = cv2.convertPointsFromHomogeneous(pos_camera)
-                pos_camera = np.array(pos_camera).ravel()
-                
-                pos = self.R@pos_camera + self.T
-                
-                if i==0:
-                    pos_old = [0,0,0]
-                    length = np.linalg.norm(pos - pos_old)
-                else: 
-                    length = length + np.linalg.norm(pos - pos_old)
-                                  
-                data_3d = np.append(pos,length)
-                
-                pos_list.append(pos)
-                data_3d_list.append(data_3d)
-                
-                pos_old = pos              
-                
-                if(plot):                
-                    plt.figure(2)
-                    plt.scatter(points_camera_1[0],points_camera_1[1],color='r') 
-                    
-            # more than one crosspoint for one epiline             
-            else:
-                
-                cam0_seg_start = i               
-                cam1_seg_start = min(sorted_indices[0:10])
-                
-                for j in range(segments):
-                    
-                    cam0_seg_end = i - 1 + int((sk_0_ordered.shape[0] - i)*(j+1)/segments)
-                    points_camera_0 = sk_0_ordered[cam0_seg_end]
-                    points_camera_0 = np.array(points_camera_0, dtype = np.float32)
-                    points_undist_0 = cv2.undistortPoints(points_camera_0, self.A0, self.dist0, P = self.A0)
-                    
-                    # Calculate epilines in camera 1 corresponding to points in camera A
-
-                    line_B = cv2.computeCorrespondEpilines(points_undist_0, 0, F) 
-                    line_B = np.array(line_B).ravel()
-                    a, b, c = line_B
-                    
-                    if (plot):
-                        plt.figure(1)
-                        plt.scatter(sk_0_ordered[cam0_seg_end, 0], sk_0_ordered[cam0_seg_end, 1],color='r')
-                        plt.pause(0.1)
-                        
-                        plt.figure(2)
-                        x_line_B = np.arange(0,self.img_1.shape[1],1)
-                        y_line_B = -(a * x_line_B  + c) / b
-                        plt.plot(x_line_B ,y_line_B,color='r' ,alpha =0.4)
-                        plt.pause(0.1)
-                        
-                    # Find intersection of epilines in camera 0
-                    distances = np.array([abs(a * x + b * y + c) / np.sqrt(a**2 + b**2) for x, y in sk_1_ordered])
-
-                    sorted_indices = np.argsort(distances)
-                    
-                    list = []
-                    for t in range(10):
-                        
-                        if sorted_indices[t] > cam1_seg_start:
-                            list.append (sorted_indices[t])
-                        
-                    cam1_seg_end = min(list)
-                    
-                    Interval = (cam1_seg_end -  cam1_seg_start - 1)/(cam0_seg_end - cam0_seg_start - 1)
-                    
-                    for k in range (cam0_seg_end - cam0_seg_start):
-                        
-                        points_camera_0 = sk_0_ordered[cam0_seg_start + k]
-                        points_camera_0 = np.array(points_camera_0, dtype = np.float32)
-                        points_undist_0 = cv2.undistortPoints(points_camera_0, self.A0, self.dist0, P = self.A0)
-                        
-                        points_camera_1 = sk_1_ordered[round(cam1_seg_start + Interval*k)]
-                        
-                        pos_camera = cv2.triangulatePoints(self.P0, self.P1, points_camera_0, points_camera_1)
-                        pos_camera = np.swapaxes(pos_camera, 0, 1)
-                        pos_camera = cv2.convertPointsFromHomogeneous(pos_camera)
-                        pos_camera = np.array(pos_camera).ravel()
-                        pos = self.R@pos_camera + self.T
-                        
-                        length = length + np.linalg.norm(pos - pos_old)
-                        data_3d = np.append(pos,length)
-                        
-                        pos_list.append(pos)
-                        data_3d_list.append(data_3d)
-                        
-                        pos_old = pos
-                        
-                    cam0_seg_start = cam0_seg_end
-                    cam1_seg_start = cam1_seg_end
-                     
-                break
-         
-        if(plot):
-            fig = plt.figure(3)
-            ax = fig.add_subplot(111, projection='3d')
-            
-            pos_list = np.array(pos_list)
-            ax.scatter(pos_list[:, 0], pos_list[:, 1], pos_list[:, 2], c='r', marker='o')
-            ax.set_xlabel('X')        
-            ax.set_ylabel('Y ')        
-            ax.set_zlabel('Z')
-            
-            ax.set_box_aspect([1, 1, 1])
-            
-        return np.stack(data_3d_list, 0 )
-       
-
+import cv2
+import math
+import numpy as np
+from scipy.io import loadmat
+from matplotlib import pyplot as plt
+from skimage.morphology import skeletonize
+from scipy.spatial.distance import cdist
+from .utils import find_longest_path
+
+#%%
+
+class EpipolarReconstructor:    
+    
+    r"""
+       Reconstruction through Epipolar geometry. 
+
+       Arguments
+       ----------
+       
+       img_0, img_1 : array
+           Photo in cam.0 and Photo in cam.1
+       
+       A0, A1, dist0, dist1, P0, P1, R, T : array
+           camera matrix
+           A0 and A1 are the intrinsic camera matrices for camera 0 and camera 1.
+           dist0 and dist1 represent the radial distortion coefficients.
+           P0 and P1 are the projection matrices for camera 0 and camera 1.
+           R stands for the rotation matrix, and T represents the translation vector.
+           
+       bin_threshold : int
+           Set pixel value greater than or equal to bin_threshold to 255 and less than bin_threshold to 0. The recommended value is 200.
+       
+       tip_estimator_params_0, tip_estimator_params_1 : store data in MATLAB
+           Defines the initial points and initial directions of the skeleton in camera 0 and camera 1.
+
+       Sources
+       ----------
+       Hartley, R., & Zisserman, A. (2004). Epipolar Geometry and the Fundamental Matrix. In Multiple View Geometry in Computer Vision (pp. 239-261). Cambridge: Cambridge University Press. doi:10.1017/CBO9780511811685.014
+    """
+    
+    def __init__(self, img_0, img_1, A0, A1, dist0, dist1, P0, P1, R, T, bin_threshold, tip_estimator_params_0, tip_estimator_params_1):
+        # Initialise variables:
+        self.img_0 = img_0 # Photo in cam.0
+        self.img_1 = img_1 # Photo in cam.1
+        
+        # camera matrix
+        self.A0 = A0 
+        self.A1 = A1 
+        self.dist0 = dist0
+        self.dist1 = dist1
+        self.P0 = P0 
+        self.P1 = P1
+        self.R = R
+        self.T = T
+        
+        self.bin_threshold = bin_threshold
+        
+        self.tip_estimator_params_0 = tip_estimator_params_0
+        self.tip_estimator_params_1 = tip_estimator_params_1
+          
+    def compute_fundamental_matrix(self, K1, K2, R, t):
+        r"""
+           By using fundamental matrix, the epipolar line in one camera can be generated from a point in anather camera. 
+           The fundamental matrix can be calculated from camera matrix using the formula (9.2) in [1]. 
+           
+           Sources
+           ----------
+           [1] Hartley, R., & Zisserman, A. (2004). Epipolar Geometry and the Fundamental Matrix. In Multiple View Geometry in Computer Vision (pp. 239-261). Cambridge: Cambridge University Press. doi:10.1017/CBO9780511811685.014
+
+         """
+        A = np.dot(K1, np.dot(R.T, t)).flatten()
+        C = np.array([[0, -A[2], A[1]], [A[2], 0, -A[0]], [-A[1], A[0], 0]])
+        ret = np.dot(np.linalg.inv(K2).T, np.dot(R, np.dot(K1.T, C)))
+        return ret
+        
+    def get_2D (self, plot = False):
+        
+        r"""
+           Obtain the skeletons of images from camera 1 and camera 2, and arrange the pixel coordinates of the skeletons in the order of the path from the starting point.
+
+           Arguments
+           ----------
+           plot : boolean
+               If True, images in camera 0 and camera 1 are displayed.
+           
+           data_cam_0, data_cam_1 : array in size (n,2), n is the number of pixels in the skeletons of images from camera 0 and camera 1.
+               The first two elements of the return value of the 'get_2D' function.
+               The 2D coordinates of each point in the skeletons of images from camera 0 and camera 1 are arranged in the order of the path from the starting point.           
+           
+           kan_img_open_0, kan_img_open_1 : array
+               The third and fourth elements of the return value of the 'get_2D' function.
+               Images in camera 0 and camera 1
+         """
+         
+        
+        # Pick the desired points for projection
+        # img in cam.0
+        if len(self.img_0.shape) == 3:
+            img = cv2.cvtColor(self.img_0, cv2.COLOR_BGR2GRAY)
+        else:
+            img = self.img_0    
+
+        param_dict = loadmat(self.tip_estimator_params_0)
+        p_start = param_dict["p_start"]
+        exit_dir = param_dict["exit_dir"]
+        
+        # filter noise
+        se = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (5,5))
+        kan_img_open_0 = cv2.morphologyEx(img, cv2.MORPH_OPEN, se)
+
+        kan_img_open_0[kan_img_open_0 >= self.bin_threshold] = 255
+        kan_img_open_0[kan_img_open_0 < self.bin_threshold] = 0
+
+        # invert the image 
+        kan_img_open_0 = 255-kan_img_open_0
+
+        # get skeleton of img0
+        img_skel = np.array(skeletonize(kan_img_open_0/255))*255
+        m,n = np.where(img_skel==255)    
+        skeleton_0 = np.array([n,m]).T
+        
+        # selekt and arrange the pixel coordinates of the skeleton_0
+        sk_0_ordered = find_longest_path(skeleton_0, p_start)
+        
+        # Remove distortion so that the epipolar line will not shift
+        sk_0_ordered = cv2.undistortPoints(sk_0_ordered.astype(np.float32), self.A0, self.dist0, P = self.A0)
+        sk_0_ordered = np.squeeze(sk_0_ordered)
+            
+        if(plot):
+            plt.figure(1)
+            plt.scatter(sk_0_ordered[:,0],sk_0_ordered[:,1])
+            plt.xlim(0, self.img_0.shape[1])
+            plt.ylim(0, self.img_0.shape[0])
+            plt.xlabel('u')
+            plt.ylabel('v')
+            plt.title('skeleton in cam.0')
+            ax = plt.gca() 
+            ax.invert_yaxis()
+               
+        # Positiondata for the skeleton in img0
+        data_cam_0 = sk_0_ordered 
+        
+        # Read img in cam.1 and skeletonize    
+        img_bgr = self.img_1
+        
+        if len(img_bgr.shape) == 3:
+            img = cv2.cvtColor(img_bgr, cv2.COLOR_BGR2GRAY)
+        else:
+            img = img_bgr
+
+        tip_estimator_params = self.tip_estimator_params_1
+        param_dict = loadmat(tip_estimator_params)
+        p_start = param_dict["p_start"]
+        exit_dir = param_dict["exit_dir"]
+        blank_idc = param_dict["blank_idc"]
+        
+        # filter noise
+        se = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (5,5))
+        kan_img_open_1 = cv2.morphologyEx(img, cv2.MORPH_OPEN, se)
+
+        kan_img_open_1[kan_img_open_1 >= self.bin_threshold] = 255
+        kan_img_open_1[kan_img_open_1 < self.bin_threshold] = 0
+
+        # invert the image 
+        kan_img_open_1 = 255-kan_img_open_1
+        
+        # get skeletion of img1
+        img_skel = np.array(skeletonize(kan_img_open_1 /255))*255
+        m,n = np.where(img_skel==255)
+        skeleton_1 = np.array([n,m]).T
+        
+        # selekt and arrange the pixel coordinates of the skeleton_1
+        sk_1_ordered = find_longest_path(skeleton_1, p_start)
+        
+        # Remove distortion, the identification of insertion point of epiplorline should be applied in undistorted image
+        sk_1_ordered = cv2.undistortPoints(sk_1_ordered.astype(np.float32), self.A1, self.dist1, P = self.A1)
+        sk_1_ordered = np.squeeze(sk_1_ordered)
+            
+        if(plot): 
+            plt.figure(2)
+            plt.scatter(sk_1_ordered[:,0],sk_1_ordered[:,1])
+            plt.xlim(0, self.img_1.shape[1])
+            plt.ylim(0, self.img_1.shape[0])
+            plt.xlabel('u')
+            plt.ylabel('v')
+            plt.title('skeleton in cam.1')
+            ax = plt.gca() 
+            ax.invert_yaxis()
+               
+        # Positiondata for the skeleton in img0
+        data_cam_1 = sk_1_ordered 
+        
+        return (data_cam_0, data_cam_1, kan_img_open_0, kan_img_open_1)
+    
+    def get_3D (self, data_cam_0=None, data_cam_1=None, interval = 20, plot=True):
+        
+        r"""
+           Obtain the 3D coordinates of the skeleton based on the 2D coordinates data in camera 0 and camera 1.
+           To establish correspondences for each point in the skeleton from camera 0 and camera 1, the points in the skeleton from camera 0 are projected into camera 1 using the fundamental matrix. 
+           The intersection points between the skeleton in camera 1 and the projection lines are identified as the corresponding points from camera 0.
+           
+           Arguments
+           ---------
+           data_cam_0, data_cam_1 : array in size (n,2), n is the number of pixels in the skeletons of images from camera 0 and camera 1.
+               The 2D coordinates of each point in the skeletons of images from camera 0 and camera 1, which arranged in the order of the path from the starting point.           
+           
+           interval : int
+               Determines how often projection lines are cast from camera 0 in camera 1 to search for corresponding points in camera 2. 
+               Increasing the interval value appropriately can reduce the algorithm's computation time.
+               
+           plot : boolean
+               If True, images in camera 0 and camera 1 as well as the 3D reconstruction, are displayed.
+         """
+        
+        # Extract rotation and translation matrices from projection matrices. Calculate fundamental matrix 
+
+        R_t_0 = np.dot(np.linalg.inv(self.A0),self.P0)
+        R_t_1 = np.dot(np.linalg.inv(self.A1),self.P1)
+
+        R0 = R_t_0[:, :3] 
+        t0 = R_t_0[:, 3] 
+        t0 = t0.reshape(-1, 1) 
+
+        R1 = R_t_1[:, :3] 
+        t1 = R_t_1[:, 3]
+        t1 = t1.reshape(-1, 1) 
+
+        R1_0 = np.dot(R1, R0.T)
+        t1_0 = np.dot(R1, -np.dot(R0.T, t0)) + t1
+
+        F = self.compute_fundamental_matrix(self.A0, self.A1, R1_0, t1_0)
+        F = np.array([[float(F[i][j]) for j in range(3)] for i in range(3)], dtype=np.float32)
+        
+        if data_cam_0.any()==None or data_cam_1.any()==None:
+            data_cam_0, data_cam_1 = self.get_2D (plot)
+            
+        else:
+            if (plot):
+                plt.figure(1)
+                plt.scatter(data_cam_0[:,0],data_cam_0[:,1])
+                plt.xlim(0, self.img_0.shape[1])
+                plt.ylim(0, self.img_0.shape[0])
+                plt.xlabel('u')
+                plt.ylabel('v')
+                plt.title('skeleton in cam.0')
+                ax = plt.gca() 
+                ax.invert_yaxis()
+                
+                plt.figure(2)
+                plt.scatter(data_cam_1[:,0],data_cam_1[:,1])
+                plt.xlim(0, self.img_1.shape[1])
+                plt.ylim(0, self.img_1.shape[0])
+                plt.xlabel('u')
+                plt.ylabel('v')
+                plt.title('skeleton in cam.1')
+                ax = plt.gca() 
+                ax.invert_yaxis()
+                                
+        sk_0_ordered = data_cam_0 [::interval]
+        sk_1_ordered = data_cam_1
+        
+        pos_list = []
+        data_3d_list = []
+
+        for i in range(sk_0_ordered.shape[0]):
+                      
+            points_camera_0 = sk_0_ordered[i]
+            
+            # Calculate epilines in camera 1 corresponding to points in camera A
+            line_B = cv2.computeCorrespondEpilines(points_camera_0[np.newaxis, :], 0, F) 
+            line_B = np.array(line_B).ravel()
+            a, b, c = line_B
+            
+            if (plot):
+                plt.figure(1)
+                plt.scatter(sk_0_ordered[i,0],sk_0_ordered[i,1],color='r')
+                plt.pause(0.1)
+                
+                plt.figure(2)
+                x_line_B = np.arange(0,self.img_1.shape[1],1)
+                y_line_B = -(a * x_line_B  + c) / b
+                plt.plot(x_line_B ,y_line_B,color='r' ,alpha =0.4)
+                plt.pause(0.1)
+                     
+            # Find intersection of epilines in camera 0
+            distances = np.array([abs(a * x + b * y + c) / np.sqrt(a**2 + b**2) for x, y in sk_1_ordered])
+
+            sorted_indices = np.argsort(distances)
+            sorted_skeleton_1 = [sk_1_ordered[i] for i in sorted_indices]
+            
+            distance = cdist(sorted_skeleton_1[0][np.newaxis, :], sorted_skeleton_1[1:10])
+            distance =  np.array(distance).ravel()
+            
+            param_dict = loadmat(self.tip_estimator_params_1)
+            p_start = param_dict["p_start"]
+            
+            if i == 0:
+                point_1_list = []
+                pre_point_1 = p_start
+                
+                for k in range(len(sorted_skeleton_1)):
+                    
+                    if cdist(sorted_skeleton_1[k][np.newaxis, :], pre_point_1) < 100:
+                        points_camera_1 = sorted_skeleton_1[k]                                          
+                        pos_camera = cv2.triangulatePoints(self.P0, self.P1, points_camera_0, points_camera_1)
+                        pos_camera = np.swapaxes(pos_camera, 0, 1)
+                        pos_camera = cv2.convertPointsFromHomogeneous(pos_camera)
+                        pos_camera = np.array(pos_camera).ravel()
+                        
+                        pos = self.R@pos_camera + self.T
+                        
+                        pos_old = [0,0,0]
+                        length = np.linalg.norm(pos - pos_old)
+                        
+                        pos_old = pos
+                        
+                        pre_point_1 = points_camera_1
+                        sorted_indices_pre = sorted_indices[k]
+                        point_1_list.append(list (points_camera_1))
+                        
+                        if (plot):
+                            plt.figure(2)
+                            plt.scatter(points_camera_1[0],points_camera_1[1],c="g")
+                        
+                        break
+            else: 
+                
+                for k in range(len(sorted_skeleton_1)):
+                    
+                    if sorted_indices_pre < 5:
+                        direction_bb = (sk_1_ordered[sorted_indices_pre+5][0]-sk_1_ordered[sorted_indices_pre][0]), (sk_1_ordered[sorted_indices_pre+5][1]-sk_1_ordered[sorted_indices_pre][1])              
+                    elif sk_1_ordered.shape[0] - sorted_indices_pre < 6:
+                        direction_bb = (sk_1_ordered[sorted_indices_pre][0]-sk_1_ordered[sorted_indices_pre-5][0]), (sk_1_ordered[sorted_indices_pre][1]-sk_1_ordered[sorted_indices_pre-5][1])              
+                    else:
+                        direction_bb = (sk_1_ordered[sorted_indices_pre+5][0]-sk_1_ordered[sorted_indices_pre-5][0]), (sk_1_ordered[sorted_indices_pre+5][1]-sk_1_ordered[sorted_indices_pre-5][1])    
+                    
+                    magnitude = math.sqrt(direction_bb[0]**2 + direction_bb[1]**2)
+                    direction_bb_unit = (direction_bb[0]/magnitude, direction_bb[1]/magnitude)
+                    
+                    direction_ziel = (sk_1_ordered[sorted_indices[k]][0]-pre_point_1[0]), (sk_1_ordered[sorted_indices[k]][1]-pre_point_1[1])
+                    magnitude = math.sqrt(direction_ziel[0]**2 + direction_ziel[1]**2)
+                    direction_ziel_unit = (direction_ziel[0]/magnitude, direction_ziel[1]/magnitude)
+                                   
+                    if cdist(sorted_skeleton_1[k][np.newaxis, :], pre_point_1[np.newaxis, :]) < 50 and np.dot(direction_bb_unit, direction_ziel_unit) > 0.8:
+                        points_camera_1 = sorted_skeleton_1[k]
+                        pre_point_1 = points_camera_1
+                        sorted_indices_pre = sorted_indices[k]
+                        point_1_list.append(list (points_camera_1))
+                        
+                        if (plot):
+                            plt.figure(2)                            
+                            plt.scatter(points_camera_1[0],points_camera_1[1],color='r')               
+                            plt.pause(0.1)                   
+                        
+                        pos_camera = cv2.triangulatePoints(self.P0, self.P1, points_camera_0, points_camera_1)
+                        pos_camera = np.swapaxes(pos_camera, 0, 1)
+                        pos_camera = cv2.convertPointsFromHomogeneous(pos_camera)
+                        pos_camera = np.array(pos_camera).ravel()
+                        
+                        pos = self.R@pos_camera + self.T
+                        
+                        length = length + np.linalg.norm(pos - pos_old)
+                        data_3d = np.append(pos,length)  
+                        
+                        pos_list.append(pos)
+                        data_3d_list.append(data_3d)
+                        
+                        pos_old = pos  
+                
+                        break    
+                
+        if(plot):
+            fig = plt.figure(3)
+            ax = fig.add_subplot(111, projection='3d')       
+            pos_list = np.array(pos_list)
+            ax.scatter(pos_list[:, 0], pos_list[:, 1], pos_list[:, 2], c='r', marker='o')
+            ax.set_xlabel('X')        
+            ax.set_ylabel('Y')        
+            ax.set_zlabel('Z')          
+            ax.set_box_aspect([1, 1, 1])
+            
+        return np.stack(data_3d_list, 0 )
+    
+    
+    def get_3D_faster (self, data_cam_0=None, data_cam_1=None, interval = 20, segments = 10, plot=True):
+        
+        r"""
+           Instead of using projection lines to establish correspondences for each point in the skeletons of images from camera 0 and camera 1, 
+           the 'get_3D_faster' method divides 'skeleton_0' and 'skeleton_1' into multiple segments, 
+           ensuring that the points within each segment in camera 0 and camera 1 correspond evenly to each other.
+           
+           Arguments
+           ---------
+           data_cam_0, data_cam_1 : array in size (n,2), n is the number of pixels in the skeletons of images from camera 0 and camera 1.
+               The 2D coordinates of each point in the skeletons of images from camera 0 and camera 1, which arranged in the order of the path from the starting point.           
+           
+           interval : int
+               Determines how often projection lines are cast from camera 0 in camera 1 to search for corresponding points in camera 2. 
+               Increasing the interval value appropriately can reduce the algorithm's computation time.
+           
+           segments : int
+               The number of segments into which the skeleton in camera 0 and camera 1 is divided.
+               
+           plot : boolean
+               If True, images in camera 0 and camera 1 as well as the 3D reconstruction, are displayed.
+         """
+        
+        # Extract rotation and translation matrices from projection matrices. Calculate fundamental matrix 
+
+        R_t_0 = np.dot(np.linalg.inv(self.A0),self.P0)
+        R_t_1 = np.dot(np.linalg.inv(self.A1),self.P1)
+
+        R0 = R_t_0[:, :3] 
+        t0 = R_t_0[:, 3] 
+        t0 = t0.reshape(-1, 1) 
+
+        R1 = R_t_1[:, :3] 
+        t1 = R_t_1[:, 3]
+        t1 = t1.reshape(-1, 1) 
+
+        R1_0 = np.dot(R1, R0.T)
+        t1_0 = np.dot(R1, -np.dot(R0.T, t0)) + t1
+
+        F = self.compute_fundamental_matrix(self.A0, self.A1, R1_0, t1_0)
+        F = np.array([[float(F[i][j]) for j in range(3)] for i in range(3)], dtype=np.float32)
+        
+        if data_cam_0.any()==None or data_cam_1.any()==None:
+            data_cam_0, data_cam_1 = self.get_2D (plot)
+            
+        else:
+            if (plot):
+                plt.figure(1)
+                plt.scatter(data_cam_0[:,0],data_cam_0[:,1])
+                plt.xlim(0, self.img_0.shape[1])
+                plt.ylim(0, self.img_0.shape[0])
+                plt.xlabel('u')
+                plt.ylabel('v')
+                plt.title('skeleton in cam.0')
+                ax = plt.gca() 
+                ax.invert_yaxis()
+                
+                plt.figure(2)
+                plt.scatter(data_cam_1[:,0],data_cam_1[:,1])
+                plt.xlim(0, self.img_1.shape[1])
+                plt.ylim(0, self.img_1.shape[0])
+                plt.xlabel('u')
+                plt.ylabel('v')
+                plt.title('skeleton in cam.1')
+                ax = plt.gca() 
+                ax.invert_yaxis()
+                
+        sk_0_ordered = data_cam_0 [::interval]
+        sk_1_ordered = data_cam_1
+        
+        pos_list = []
+        data_3d_list = []       
+
+        for i in range(sk_0_ordered.shape[0]):
+                     
+            points_camera_0 = sk_0_ordered[i]
+            points_camera_0 = np.array(points_camera_0, dtype = np.float32)
+            points_undist_0 = cv2.undistortPoints(points_camera_0, self.A0, self.dist0, P = self.A0)
+            
+            # Calculate epilines in camera 1 corresponding to points in camera A
+            line_B = cv2.computeCorrespondEpilines(points_undist_0, 0, F) 
+            line_B = np.array(line_B).ravel()
+            a, b, c = line_B
+            
+            if (plot):
+                plt.figure(1)
+                plt.scatter(sk_0_ordered[i,0],sk_0_ordered[i,1],color='r')
+                plt.pause(0.1)
+                
+                plt.figure(2)
+                x_line_B = np.arange(0,self.img_1.shape[1],1)
+                y_line_B = -(a * x_line_B  + c) / b
+                plt.plot(x_line_B ,y_line_B,color='r' ,alpha =0.4)
+                plt.pause(0.1)
+                    
+            # Find intersection of epilines in camera 0
+            distances = np.array([abs(a * x + b * y + c) / np.sqrt(a**2 + b**2) for x, y in sk_1_ordered])
+
+            sorted_indices = np.argsort(distances)
+            sorted_skeleton_1 = [sk_1_ordered[i] for i in sorted_indices]
+            
+            distance = cdist(sorted_skeleton_1[0][np.newaxis, :], sorted_skeleton_1[1:10])
+            distance =  np.array(distance).ravel()
+            
+            # only one crosspoint for one epiline
+            if max (distance) < 20:
+                
+                points_camera_1 = sorted_skeleton_1[0]                      
+                pos_camera = cv2.triangulatePoints(self.P0, self.P1, points_camera_0, points_camera_1)
+                pos_camera = np.swapaxes(pos_camera, 0, 1)
+                pos_camera = cv2.convertPointsFromHomogeneous(pos_camera)
+                pos_camera = np.array(pos_camera).ravel()
+                
+                pos = self.R@pos_camera + self.T
+                
+                if i==0:
+                    pos_old = [0,0,0]
+                    length = np.linalg.norm(pos - pos_old)
+                else: 
+                    length = length + np.linalg.norm(pos - pos_old)
+                                  
+                data_3d = np.append(pos,length)
+                
+                pos_list.append(pos)
+                data_3d_list.append(data_3d)
+                
+                pos_old = pos              
+                
+                if(plot):                
+                    plt.figure(2)
+                    plt.scatter(points_camera_1[0],points_camera_1[1],color='r') 
+                    
+            # more than one crosspoint for one epiline             
+            else:
+                
+                cam0_seg_start = i               
+                cam1_seg_start = min(sorted_indices[0:10])
+                
+                for j in range(segments):
+                    
+                    cam0_seg_end = i - 1 + int((sk_0_ordered.shape[0] - i)*(j+1)/segments)
+                    points_camera_0 = sk_0_ordered[cam0_seg_end]
+                    points_camera_0 = np.array(points_camera_0, dtype = np.float32)
+                    points_undist_0 = cv2.undistortPoints(points_camera_0, self.A0, self.dist0, P = self.A0)
+                    
+                    # Calculate epilines in camera 1 corresponding to points in camera A
+
+                    line_B = cv2.computeCorrespondEpilines(points_undist_0, 0, F) 
+                    line_B = np.array(line_B).ravel()
+                    a, b, c = line_B
+                    
+                    if (plot):
+                        plt.figure(1)
+                        plt.scatter(sk_0_ordered[cam0_seg_end, 0], sk_0_ordered[cam0_seg_end, 1],color='r')
+                        plt.pause(0.1)
+                        
+                        plt.figure(2)
+                        x_line_B = np.arange(0,self.img_1.shape[1],1)
+                        y_line_B = -(a * x_line_B  + c) / b
+                        plt.plot(x_line_B ,y_line_B,color='r' ,alpha =0.4)
+                        plt.pause(0.1)
+                        
+                    # Find intersection of epilines in camera 0
+                    distances = np.array([abs(a * x + b * y + c) / np.sqrt(a**2 + b**2) for x, y in sk_1_ordered])
+
+                    sorted_indices = np.argsort(distances)
+                    
+                    list = []
+                    for t in range(10):
+                        
+                        if sorted_indices[t] > cam1_seg_start:
+                            list.append (sorted_indices[t])
+                        
+                    cam1_seg_end = min(list)
+                    
+                    Interval = (cam1_seg_end -  cam1_seg_start - 1)/(cam0_seg_end - cam0_seg_start - 1)
+                    
+                    for k in range (cam0_seg_end - cam0_seg_start):
+                        
+                        points_camera_0 = sk_0_ordered[cam0_seg_start + k]
+                        points_camera_0 = np.array(points_camera_0, dtype = np.float32)
+                        points_undist_0 = cv2.undistortPoints(points_camera_0, self.A0, self.dist0, P = self.A0)
+                        
+                        points_camera_1 = sk_1_ordered[round(cam1_seg_start + Interval*k)]
+                        
+                        pos_camera = cv2.triangulatePoints(self.P0, self.P1, points_camera_0, points_camera_1)
+                        pos_camera = np.swapaxes(pos_camera, 0, 1)
+                        pos_camera = cv2.convertPointsFromHomogeneous(pos_camera)
+                        pos_camera = np.array(pos_camera).ravel()
+                        pos = self.R@pos_camera + self.T
+                        
+                        length = length + np.linalg.norm(pos - pos_old)
+                        data_3d = np.append(pos,length)
+                        
+                        pos_list.append(pos)
+                        data_3d_list.append(data_3d)
+                        
+                        pos_old = pos
+                        
+                    cam0_seg_start = cam0_seg_end
+                    cam1_seg_start = cam1_seg_end
+                     
+                break
+         
+        if(plot):
+            fig = plt.figure(3)
+            ax = fig.add_subplot(111, projection='3d')
+            
+            pos_list = np.array(pos_list)
+            ax.scatter(pos_list[:, 0], pos_list[:, 1], pos_list[:, 2], c='r', marker='o')
+            ax.set_xlabel('X')        
+            ax.set_ylabel('Y ')        
+            ax.set_zlabel('Z')
+            
+            ax.set_box_aspect([1, 1, 1])
+            
+        return np.stack(data_3d_list, 0 )
+       
+
```

### Comparing `icpReconstructor-0.1.0/icpReconstructor/torch_reconstruction.py` & `icpReconstructor-0.1.1/icpReconstructor/torch_reconstruction.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,839 +1,839 @@
-# -*- coding: utf-8 -*-
-"""
-This script contains a PyTorch-based implementation of the continuum robot reconstruction algorithm presented in xxx.
-The package needs a PyTorch build with LAPACK/BLAS, the easiest way for getting this is by installing PyTorch using Conda/Anaconda.
-"""
-
-import torch
-import torch.nn as nn
-import numpy as np
-from .utils import fromWorld2Img, ball_tree_norm, PixelDataset
-from abc import ABC, abstractmethod
-from torchdiffeq import odeint as odeint
-from torch.utils.data import DataLoader
-from tqdm import tqdm
-from warnings import warn
-from copy import deepcopy
-
-
-class TorchParameterizedFunction(nn.Module, ABC):
-    """
-        Class for storing parameterized functions for usage with TorchMovingFrame.
-        Can also be used for other models like polynomials, but it's original purpose was the
-        usage as curvature polynomials.
-    """
-
-    @abstractmethod
-    def get_u_fun( self, idx, s0, s1 ):
-        pass
-
-
-class Polynomial3Torch(TorchParameterizedFunction):
-    r"""
-        Parameterization of degree 3 polynomials. The parameters are the function value and the derivative at start and end.
-        This, for example, allows for easy initialization given simulation results from physics-based models.
-
-        .. note::
-            The parameters for the polynomials are given as
-            :math:`up(i,:) = [f(l[i-1]), f'(l[i-1]), f(l[i]), f'(l[i])]`
-
-        Arguments
-        ----------
-        n : int
-            Number of polynomials used to approximate the cr. Typically set to the number of tubes.
-
-        u_p : str or n-by-4 tensor
-            Optional initialization of the curvature parameters.
-
-        continuous : boolean
-            If True, the polynomials are forced to be continuous.
-
-        random_init : boolean
-            If True and u_p is None, the parameters are initialized randomly.
-
-        end_no_curvature : boolean
-            If True, the last polynomial is forced to be 0. This allows for physically more reasonable uz, so
-            :math:`f_n(s) = 0`
-    """
-
-    def __init__( self, n, u_p=None, optimize=True, continuous=False, random_init=False, end_no_curvature=False ):
-        super().__init__()
-        self.n = n
-        if u_p is not None:
-            _u_p = u_p.clone().detach()
-        if continuous and optimize:
-            n_f = n - end_no_curvature * 2 + 1
-            n_f_dot = n - end_no_curvature
-            if u_p is None:
-                self.u_params = nn.Parameter(10 * (torch.rand(n_f, 1) - 0.5) if random_init else torch.zeros(n_f, 1))
-                self.u_dot_params = nn.Parameter(10 * (torch.rand(n_f_dot, 2) - 0.5) if random_init else torch.zeros(n_f_dot, 2))
-                u_node = torch.concatenate((self.u_params, torch.zeros(2, 1)), 0) if end_no_curvature else self.u_params
-                u_dot_node = torch.concatenate((self.u_dot_params, torch.zeros(1, 2)), 0) if end_no_curvature else self.u_dot_params
-            else:
-                self.u_params = nn.Parameter(torch.cat((_u_p[:, 0, None], _u_p[-1, 2, None, None]), 0))
-                self.u_dot_params = nn.Parameter(_u_p[:, 1::2])
-                u_node = torch.concatenate((self.u_params, torch.zeros(2, 1)), 0) if end_no_curvature else self.u_params
-                u_dot_node = torch.concatenate((self.u_dot_params, torch.zeros(1, 2)), 0) if end_no_curvature else self.u_dot_params
-            self.u_p = torch.concatenate((u_node[:-1, :], u_dot_node[:, 0, None], u_node[1:, :], u_dot_node[:, 1, None]), 1)
-        else:
-            if u_p is None and optimize:
-                self.u_p = nn.Parameter(10 * (torch.rand(n, 4) - 0.5) if random_init else torch.zeros(n, 4))
-            elif u_p is None and not optimize:
-                self.register_buffer('u_p', torch.zeros(n, 4))
-            elif optimize:
-                self.u_p = nn.Parameter(_u_p)
-            else:
-                self.register_buffer('u_p', _u_p)
-
-    def get_u_fun( self, idx, s0, s1 ):
-        r"""
-            Function for generating the degree 3 polynomial from the curvature parameters.
-            u_p = [f(s0), f'(s0), f(s1), f'(s1)]
-        """
-        u_p = self.u_p[idx, :]
-        T = s1 - s0
-        a = (2 * u_p[0] - 2 * u_p[2] + T * u_p[1] + T * u_p[3]) / (T ** 3)
-        b = -(3 * u_p[0] - 3 * u_p[2] + 2 * T * u_p[1] + T * u_p[3]) / (T ** 2)
-        c = u_p[1]
-        d = u_p[0]
-
-        def u_fun( s ):
-            return torch.stack([d, c, b, a]) @ ((s - s0) ** (torch.arange(0, 4)).reshape(4, 1))
-
-        return u_fun
-
-
-class PolynomialKTorch(TorchParameterizedFunction):
-    r"""
-        Parameterization of degree K polynomials for the curvatures used by TorchMovingFrame.
-
-        Arguments
-        ----------
-        n : int
-            Number of polynomials used to approximate the cr. Typically set to the number of tubes.
-
-        K : int
-            Degree used for the polynomials.
-
-        u_p : str or n-by-K tensor
-            Optional initialization of the curvature parameters.
-
-        optimize : boolean
-            If True, the parameters are optimized during the fitting process.
-
-        random_init : boolean
-            If True and u_p is None, the parameters are initialized randomly.
-
-        end_no_curvature : boolean
-            If True, the last polynomial is forced to be 0. This allows for physically more reasonable uz, so
-    """
-
-    def __init__( self, n, K, u_p=None, optimize=True, random_init=False, end_no_curvature=False ):
-        super().__init__()
-        self.n = n
-        self.K = K
-        if u_p is not None:
-            _u_p = u_p.clone().detach()
-        if optimize:
-            n_f = n - end_no_curvature
-            if u_p is None:
-                self.u_params = nn.Parameter(10 * (torch.rand(n_f, K + 1) - 0.5) if random_init else torch.zeros(n_f, K + 1))
-            else:
-                self.u_params = nn.Parameter(_u_p[:n_f, :])
-            self.u_p = torch.concatenate((self.u_params, torch.zeros(1, K + 1)), 0) if end_no_curvature else self.u_params
-        else:
-            if u_p is None:
-                self.register_buffer('u_p', torch.zeros(n, K + 1))
-            else:
-                self.register_buffer('u_p', _u_p)
-
-    def get_u_fun( self, idx, s0, s1 ):
-        '''
-            Function for generating the K-th-ordner polynomial from the curvature parameters.
-        '''
-
-        def u_fun( s ):
-            return self.u_p[idx, :] @ (((s - s0)/(s1 - s0)) ** (torch.arange(0, self.K + 1)).reshape(self.K + 1, 1))
-
-        return u_fun
-
-def __curvature_matrix_rotm( ux, uy, uz ):
-    null = torch.zeros([1])
-    elems = [[null, null, uy], [uz, null, null], [null, ux, null]]
-    curvature_mat = torch.stack([torch.concatenate(i, 0) for i in elems], 0)
-    return curvature_mat - curvature_mat.T
-
-def __curvature_matrix_quat( ux, uy, uz ):
-    null = torch.zeros([1])
-    elems = [[null, null, null, null], [ux, null, uz, null], [uy, null, null, ux],[uz, uy, null, null]]
-    curvature_mat = torch.stack([torch.concatenate(i, 0) for i in elems], 0)
-    return curvature_mat - curvature_mat.T
-
-CURVATURE_FCN = {'rotm':__curvature_matrix_rotm, 'quat':__curvature_matrix_quat}
-
-class TorchPolynomialCurve(nn.Module):
-    """
-        NOTE: It is not recommended to use this class. It was developed for research purposes, so it is kept for reference.
-        This class implements the a direct polynomial formulation for reconstructing a continuum robot's backbone.
-        The parameterization of the curvatures ux, uy, and uz is achieved by providing TorchParameterizedFunction objects.
-
-        Arguments
-        ----------
-        l : tensor
-            List of the lengths up to which the corresponding polynomial is used. Is
-            typically selected to be each NiTi tube's length outside of the actuation
-            unit.
-
-        p0 : 3-by-1 tensor
-            A 3D point where the CR exits the actuation unit in world
-            coordinates.
-
-        p0_parametric : boolean
-            If True, the initial position p0 is estimated as well.
-
-        ux : n-by-4 tensor or TorchParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the x-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        uy : n-by-4 tensor or TorchParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the y-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        uz : n-by-4 tensor or TorchParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the z-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        optimize : list of 3 booleans
-            If True, the corresponding curvature [ ux, uy, uz ] is optimized during the fitting process. Only used if the 
-            corresponding curvature is not given as a TorchParameterizedFunction object.
-
-        continuous_u : list of 3 booleans
-            If true, the corresponding curvature [ ux, uy, uz ] is enforced to be continuous. Only used if the 
-            corresponding curvature is not given as a TorchParameterizedFunction object.
-
-        random_init : list of 3 booleans
-            If true, the corresponding curvature [ ux, uy, uz ] is randomly initialized. Only used if the 
-            corresponding curvature is not given as a TorchParameterizedFunction object.
-
-    """
-    
-    def __init__(
-            self, l, p0=torch.zeros(3, 1), p0_parametric=False, 
-            ux=None, uy=None, uz=None, optimize=[True, True, True], continuous_u=[True, True, True], 
-            random_init=[False] * 3 
-            ):
-        super().__init__()
-        
-        self.ux_funs, self.uy_funs, self.uz_funs = None, None, None
-
-        self.l = l
-        self.n = len(l)
-        
-        if p0_parametric:
-            self.p0 = nn.Parameter(p0)
-        else:
-            self.p0 = p0
-            
-        if issubclass(type(ux), TorchParameterizedFunction):  # Check if ux is already a TorchParameterizedFunction.
-            self.ux = ux
-        else:  # If not, initialize it as a Polynomial3Torch.
-            self.ux = Polynomial3Torch(self.n, ux, optimize=optimize[0], continuous=continuous_u[0], random_init=random_init[0])
-
-        if issubclass(type(uy), TorchParameterizedFunction):  # Check if uy is already a TorchParameterizedFunction.
-            self.uy = uy
-        else:  # If not, initialize it as a Polynomial3Torch.
-            self.uy = Polynomial3Torch(self.n, uy, optimize=optimize[1], continuous=continuous_u[1], random_init=random_init[1])
-
-        if issubclass(type(uz), TorchParameterizedFunction):  # Check if uz is already a TorchParameterizedFunction.
-            self.uz = uz
-        else:  # If not, initialize it as a Polynomial3Torch.
-            self.uz = Polynomial3Torch(self.n, uz, optimize=optimize[2], continuous=continuous_u[2], random_init=random_init[2])
-
-        self.set_funs()
-        
-    def set_funs( self ):
-        """
-            Function that fills the curvature function handles. Has to be called after each optimizer step.
-        """
-        self.ux_funs = [self.ux.get_u_fun(0, 0, self.l[0])]
-        self.uy_funs = [self.uy.get_u_fun(0, 0, self.l[0])]
-        self.uz_funs = [self.uz.get_u_fun(0, 0, self.l[0])]
-
-        for i in range(1, self.n):
-            self.ux_funs.append(self.ux.get_u_fun(i, self.l[i - 1], self.l[i]))
-            self.uy_funs.append(self.uy.get_u_fun(i, self.l[i - 1], self.l[i]))
-            self.uz_funs.append(self.uz.get_u_fun(i, self.l[i - 1], self.l[i]))
-            
-    def forward( self, s_val ):
-        """
-        TODO: Something about this is off, but I cannot figure out what it is.
-        """
-        for i in range(len(self.l)):
-            s = s_val[(s_val <= self.l[i]) & ((self.l[i-1] if i >= 1 else 0) <= s_val)]
-            if i == 0:
-                p = torch.stack([self.ux_funs[i](s), self.uy_funs[i](s), self.uz_funs[i](s)], 0)
-            else:
-                p = torch.stack([self.ux_funs[i](s), self.uy_funs[i](s), self.uz_funs[i](s)], 0)
-        
-        return p.T
-
-
-class TorchMovingFrame(nn.Module):
-    """
-        This class implements the moving frame formulation for reconstructing a continuum robot's backbone.
-        The parameterization of the curvatures ux, uy, and uz is achieved by providing TorchParameterizedFunction objects.
-
-        Arguments
-        ----------
-        l : tensor
-            List of the lengths up to which the corresponding polynomial is used. Is
-            typically selected to be each NiTi tube's length outside of the actuation
-            unit.
-
-        p0 : 3-by-1 tensor
-            A 3D point where the CR exits the actuation unit in world
-            coordinates.
-
-        p0_parametric : boolean
-            If True, the initial position p0 is estimated as well.
-
-        R0 : 3-by-3 or 4-by-1 tensor
-            Either a 3-by-3 matrix from SO(3) that describes the orientation of
-            the exiting CR (ref. [1]) or, if R0_parametric is True, tensor of
-            shape (4,). The matrix is then parametrized using quaternions.
-
-        R0_parametric : boolean
-            If True, the initial orientation R0 is estimated as well. To ensure
-            that R0 remains inside SO(3), it is parameterized using quaternions.
-
-        ux : n-by-4 tensor or TorchParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the x-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        uy : n-by-4 tensor or TorchParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the y-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        uz : n-by-4 tensor or TorchParameterizedFunction
-            Initial guess for the parameters of the polynomials
-            for the z-curvatures of the n polynomials. If set to None it is either initialized
-            as 0s or uniformly distributed between -5 and 5 if random_init is True.
-
-        optimize : list of 3 booleans
-            If True, the corresponding curvature [ ux, uy, uz ] is optimized during the fitting process. Only used if the 
-            corresponding curvature is not given as a TorchParameterizedFunction object.
-
-        integrator : str
-            Integration method from the following list:
-
-                - "midpoint"
-                - "rk4"
-                - "dopri5",
-                - "bost3"
-                - "fehlberg2"
-                - "adaptive_heun"
-                - "euler"
-                - "dopri8"
-                - "explicit_adams"
-                - "implicit_adams"
-
-            The midpoint rule typically gives a good trade-off between accuracy and speed.
-
-        continuous_u : list of 3 booleans
-            If true, the corresponding curvature [ ux, uy, uz ] is enforced to be continuous. Only used if the 
-            corresponding curvature is not given as a TorchParameterizedFunction object.
-
-        random_init : list of 3 booleans
-            If true, the corresponding curvature [ ux, uy, uz ] is randomly initialized. Only used if the 
-            corresponding curvature is not given as a TorchParameterizedFunction object.
-
-        Sources
-        ----------
-        [1] 10.1109/TRO.2010.2062570, Rucker, D. Caleb, Bryan A. Jones, and Robert J. Webster III. "A geometrically exact model for externally loaded concentric-tube continuum robots." IEEE transactions on robotics 26.5 (2010): 769-780.
-    """
-
-    def __init__(
-            self, l, p0=torch.zeros(3, 1), p0_parametric=False, R0=None, R0_parametric=False, rotation_method="rotm", 
-            ux=None, uy=None, uz=None, optimize=[True, True, False], integrator='midpoint', continuous_u=[False, False, True], 
-            random_init=[False] * 3 
-            ):
-        super().__init__()
-
-        self.__integrator = 'midpoint'
-        self.__previous_integrate_parameters = None
-        self.ux_funs, self.uy_funs, self.uz_funs = None, None, None
-        self.rotation_method = rotation_method
-
-        self.l = l
-        self.n = len(l)
-
-        if p0_parametric:
-            self.p0 = nn.Parameter(p0)
-        else:
-            self.p0 = p0
-        
-        if R0 is None:
-            if rotation_method == "quat" or R0_parametric:
-                R0 = torch.tensor([1, 0, 0, 0])
-            else:
-                R0 = torch.eye(3)
-        
-        if R0_parametric:
-            # If R0 is parametric, it is assumed to be a quaternion. The quaternion is then normalized and converted to a rotation matrix.
-            if R0.shape != torch.Size([4, ]):
-                raise Exception("If R0_parametric is set to true, the input R0 is considered to be a quaternion, so its shape is supposed to be (4,).")
-            _R0 = R0.float()
-            self.q = nn.Parameter(_R0 / torch.linalg.vector_norm(_R0))
-            q = self.q / torch.linalg.vector_norm(self.q)  # Setup the quaternion.
-            
-            if rotation_method == "quat":
-                self.R0 = q
-            else:
-                self.R0 = torch.zeros((3, 3))
-                # Convert the quaternion to a rotation matrix R0.
-                self.R0[0, 0] = 1 - 2 * (q[2] ** 2 + q[3] ** 2)
-                self.R0[0, 1] = 2 * (q[1] * q[2] - q[0] * q[3])
-                self.R0[0, 2] = 2 * (q[1] * q[3] + q[0] * q[2])
-                self.R0[1, 0] = 2 * (q[1] * q[2] + q[0] * q[3])
-                self.R0[1, 1] = 1 - 2 * (q[1] ** 2 + q[3] ** 2)
-                self.R0[1, 2] = 2 * (q[2] * q[3] - q[0] * q[1])
-                self.R0[2, 0] = 2 * (q[1] * q[3] - q[0] * q[2])
-                self.R0[2, 1] = 2 * (q[2] * q[3] + q[0] * q[1])
-                self.R0[2, 2] = 1 - 2 * (q[1] ** 2 + q[2] ** 2)
-        else:
-            self.R0 = R0
-        
-        self.x0 = torch.cat((self.p0.flatten(), self.R0.flatten()), 0)
-        self.integrator = integrator
-        self.ode_solution = None
-        self.ode = self.__quat_ode if rotation_method == "quat" else self.__rotm_ode
-        self.curvature_mat_fcn = CURVATURE_FCN[rotation_method]
-
-        if issubclass(type(ux), TorchParameterizedFunction):  # Check if ux is already a TorchParameterizedFunction.
-            self.ux = ux
-        else:  # If not, initialize it as a Polynomial3Torch.
-            self.ux = Polynomial3Torch(self.n, ux, optimize=optimize[0], continuous=continuous_u[0], random_init=random_init[0])
-
-        if issubclass(type(uy), TorchParameterizedFunction):  # Check if uy is already a TorchParameterizedFunction.
-            self.uy = uy
-        else:  # If not, initialize it as a Polynomial3Torch.
-            self.uy = Polynomial3Torch(self.n, uy, optimize=optimize[1], continuous=continuous_u[1], random_init=random_init[1])
-
-        if issubclass(type(uz), TorchParameterizedFunction):  # Check if uz is already a TorchParameterizedFunction.
-            self.uz = uz
-        else:  # If not, initialize it as a Polynomial3Torch.
-            self.uz = Polynomial3Torch(self.n, uz, optimize=optimize[2], continuous=continuous_u[2], random_init=random_init[2])
-
-        self.set_funs()  # Fill the curvature function handles.
-
-    def set_funs( self ):
-        """
-            Function that fills the curvature function handles. Has to be called after each optimizer step.
-        """
-        self.ux_funs = [self.ux.get_u_fun(0, 0, self.l[0])]
-        self.uy_funs = [self.uy.get_u_fun(0, 0, self.l[0])]
-        self.uz_funs = [self.uz.get_u_fun(0, 0, self.l[0])]
-
-        for i in range(1, self.n):
-            self.ux_funs.append(self.ux.get_u_fun(i, self.l[i - 1], self.l[i]))
-            self.uy_funs.append(self.uy.get_u_fun(i, self.l[i - 1], self.l[i]))
-            self.uz_funs.append(self.uz.get_u_fun(i, self.l[i - 1], self.l[i]))
-
-    @property
-    def integrator( self ):
-        return self.__integrator
-
-    @integrator.setter
-    def integrator( self, value ):
-        if value not in ["midpoint", "rk4", "dopri5", "bosh3", "fehlberg2", "adaptive_heun", "euler", "dopri8", "explicit_adams", "implicit_adams"]:
-            raise Exception(
-                "The given integrator is not valid or available. Please use one of the solvers given by the torchdiffeq package: https://github.com/rtqichen/torchdiffeq")
-        if value != self.__integrator:
-            """
-                Ensure that the integration is run again after the integrator was changed.
-            """
-            self.__previous_integrate_parameters = None
-        self.__integrator = value
-
-    def u_hat( self, s ):
-        """
-            Function for transforming u_p to the necessary skew-symmstric matrix. idx_fun is the index of the curvature function that is active at the current
-            arc-length.
-        """
-        if s <= self.l[-1]:
-            active_tube_idx = torch.where(self.l >= s)[0]
-            idx_fun = torch.min(active_tube_idx)
-        else:
-            idx_fun = self.n - 1
-
-        ux, uy, uz = self.ux_funs[idx_fun](s), self.uy_funs[idx_fun](s), self.uz_funs[idx_fun](s)
-        curvature_mat = self.curvature_mat_fcn( ux, uy, uz )
-        return curvature_mat
-    
-    def forward( self, s_val ):
-        return self.integrate(s_val)[:,:3]
-    
-    def integrate( self, s_val ):
-        """
-            Get the solution of the integration. Integration is only performed if the previous (curvature) parameters did change or if
-            the integration scheme changed.
-
-            Arguments:
-            ----------
-            s_val : tensor, optional
-                If values for the arc-length are given, the integration scheme is evaluated at these points and not the
-                ones used in the integration. This is useful for plotting the solution. If None, the arc-lengths used in the integration.
-        """
-        if self.__previous_integrate_parameters is None or (list(self.__previous_integrate_parameters()) == list(self.parameters())):            
-            self.ode_solution = odeint(self.ode, self.x0, s_val, method=self.integrator)
-        return self.ode_solution
-       
-    def __quat_ode( self, s, x ):
-        """
-            Right-hand side of the quaternion moving frame ODE.
-
-            Arguments
-            ----------
-            s : float
-                The current value of the arc-length.
-
-            x : 7-by-1 float tensor
-                The current state x = [p, q]. p is the position of the CR in world coordinates and q is the quaternion describing the orientation of the
-                CR at the current arc-length.
-        """
-        q = x[3:]
-        dp1 = (q[1]*q[3]+q[0]*q[2])
-        dp2 = (q[2]*q[3]-q[0]*q[1])
-        dp3 = (-q[1]**2-q[2]**2)
-        dp = torch.tensor([0,0,1])+2*torch.stack([dp1, dp2, dp3])/(torch.sum(q**2))
-        dq = self.u_hat(s)@q/2
-        return torch.concat((dp, dq), 0)
-    
-    def __rotm_ode( self, s, x ):
-        """
-            Right-hand side of the moving frame ODE.
-
-            Arguments
-            ----------
-            s : float
-                The current value of the arc-length.
-
-            x : 12-by-1 float tensor
-                The current state x = [p, R]. p is the position of the CR in world coordinates and R is the rotation matrix describing the orientation of the
-                CR at the current arc-length.
-        """
-        R = x[3:].reshape((3, 3))
-
-        dp = R[:, 2].flatten()
-        dR = (R @ self.u_hat(s)).flatten()
-        return torch.concat((dp, dR), 0)
-    
-
-class TorchCurveEstimator():
-    r"""
-        This class implements the PyTorch-based curve estimator (TCE) for continuum robots.
-        The TCE takes a parameterized model for the continuum robot - this can be a rotation
-        frame, circular arcs, differentiable rendering model, ... - and optimizes for the
-        torch.parameters using an Iterative Closest Point algorithm.
-
-        Arguments
-        ----------
-        curve_model : nn.Module
-            PyTorch model that parameterizes the reconstruction of thecontinuum robot. The model has to be
-            callable with the arc-length as the only argument.
-        
-        l : positive scalar
-            The length of the continuum robot from the starting position to the tip of the robot.
-
-        camera_calibration_parameters : list of dictionaries
-            A list of dictionaries containing the keys
-            "A", "dist", "P", "R", and "T". The function "camera_folder_to_params" can
-            automatically generate this list for you.
-
-        n_steps : int
-            Number of intermediate steps to evaluate the reconstructed cr at.
-            If low, the computation is fast, but for very low values the convergence might
-            be bad. If high, a better solution might be found, at cost of higher computation
-            times.
-
-        w : double
-            Weighting of the two cost functions. 0 (only track distance of pixels to
-            reconstruction) is typically a good value, but if parts of the cr are occluded,
-            increasing w can help.
-
-        dist_norm : int
-            Order of the metric used to penalize distances. Higher values give more cost to big errors.
-    """
-    
-    def __init__(self, curve_model, camera_calibration_parameters, l, w=0., n_steps=50, dist_norm=2, post_step_cb=[], post_epoch_cb=[] ):
-        super().__init__()
-        assert isinstance(curve_model, nn.Module), "The curve_model needs to be an instance of nn.Module" 
-        self.camera_calibration_parameters = camera_calibration_parameters
-        self.curve_model = curve_model
-        self.l = l
-        
-        self.w = w
-        self.n_steps = n_steps
-        self.dist_norm = dist_norm
-        self.pixel_diff_state = None
-        self.backbone_diff_state = None
-        self.__bb_pixel_coordinates = None
-        if len(camera_calibration_parameters) < 2:
-            warn("Two or more images are necessary for a successful reconstruction.")
-        self.camera_calibration_parameters = camera_calibration_parameters
-        self.s_val = torch.linspace(0, self.l, self.n_steps)
-        self.reset_diff_states()
-        self.post_step_cb = post_step_cb
-        self.post_epoch_cb = post_epoch_cb
-
-    def get_img_coordinates( self ):
-        """
-            Project the computed backbone points to all the images and return the image coordinates.
-        """
-        if self.__bb_pixel_coordinates is None:
-            backbone_pts = self.curve_model(self.s_val).T
-            self.__bb_pixel_coordinates = []
-            for i in range(len(self.camera_calibration_parameters)):
-                self.__bb_pixel_coordinates.append(fromWorld2Img(backbone_pts, **self.camera_calibration_parameters[i]).T)
-        return self.__bb_pixel_coordinates
-
-    def reset_diff_states( self ):
-        """
-            Reset the diff states, so that in the next call off get_*_diff_idx, the correspondances are computated agian.
-        """
-        self.pixel_diff_state = None
-        self.backbone_diff_state = None
-
-    def get_pixel_diff_idx( self, cr_img_coordinates, img_idx_data ):
-        """
-            Computes for each CR pixel the index of the closest reconstruction pixel.
-
-            Arguments
-            ----------
-            cr_img_coordinates : m-by-2 int
-                Coordinates of CR pixels in image coordinates.
-
-            img_idx_data : m-by-1 int
-                Vector containing the index from which image the corresponding img_coordinates entry was taken.
-        """
-        backbone_img_coordinates = self.get_img_coordinates()
-        if self.pixel_diff_state is None:
-            idx_min_dist = []
-            cr_img_coordinates_sorted = []
-            for i in np.unique(np.unique(img_idx_data)):
-                cr_img_coordinates_i = cr_img_coordinates[img_idx_data == i, :]
-                # _, idc_min = brute_force_distance_norm(cr_img_coordinates_i.float(), backbone_img_coordinates[i], p=self.dist_norm)
-                idc_min = ball_tree_norm(cr_img_coordinates_i.float(), backbone_img_coordinates[i], p=self.dist_norm)
-                idx_min_dist.append(idc_min)
-                cr_img_coordinates_sorted.append(cr_img_coordinates_i)
-            self.pixel_diff_state = dict(idx_min_dist=idx_min_dist, cr_img_coordinates_sorted=cr_img_coordinates_sorted)
-        
-        return self.pixel_diff_state["idx_min_dist"], self.pixel_diff_state["cr_img_coordinates_sorted"]
-
-    def pixel_diff( self, cr_img_coordinates, img_idx_data ):
-        """
-            Compute the distance of each CR pixel to the closest reconstruction point in image coordinates.
-
-            Arguments
-            ----------
-            cr_img_coordinates : m-by-2 tensor
-                Tensor containing the image coordinates of CR pixels.
-
-            img_idx_data :m-by-1 tensor
-                Tensor containing the index of the image a point was taken from.
-       """
-        curve_pixel_coordinates = self.get_img_coordinates()
-        diffs = None
-        idx_min_dist, cr_img_coordinates_sorted = self.get_pixel_diff_idx(cr_img_coordinates, img_idx_data)
-        for i in np.unique(img_idx_data):
-            diffs = curve_pixel_coordinates[i][idx_min_dist[i], :] - cr_img_coordinates_sorted[i] if diffs is None else torch.concatenate(
-                (diffs, curve_pixel_coordinates[i][idx_min_dist[i], :] - cr_img_coordinates_sorted[i]), 0)
-        return diffs
-
-    def pixel_loss( self, cr_img_coordinates, img_idx_data ):
-        """
-            Computes the average distance of each CR pixel to the corresponding backbone point.
-        """
-        # Penalizes the minimum distance of each measurement point to the reconstructed curve.
-        return torch.linalg.vector_norm(self.pixel_diff(cr_img_coordinates, img_idx_data), self.dist_norm, 1).mean()  # **self.dist_norm
-
-    def get_backbone_diff_idx( self, cr_img_coordinates, img_idx_data ):
-        """
-            Computes for each backbone point in image coordinates the index of the closest CR pixel .
-
-            Arguments
-            ----------
-            cr_img_coordinates : m-by-2 int
-                Coordinates of CR pixels in image coordinates.
-
-            img_idx_data : m-by-1 int
-                Vector containing the index from which image the corresponding img_coordinates entry was taken.
-
-        """
-        backbone_img_coordinates = self.get_img_coordinates()
-        if self.backbone_diff_state is None:
-            idx_min_dist = []
-            cr_img_coordinates_sorted = []
-            for i in np.unique(np.unique(img_idx_data)):
-                cr_img_coordinates_i = cr_img_coordinates[img_idx_data == i, :]
-                # _, idc_min = brute_force_distance_norm(backbone_img_coordinates[i], cr_img_coordinates_i.float(), p=self.dist_norm)
-                idc_min = ball_tree_norm(backbone_img_coordinates[i], cr_img_coordinates_i.float(), p=self.dist_norm)
-                idx_min_dist.append(idc_min)
-                cr_img_coordinates_sorted.append(cr_img_coordinates_i)
-            self.backbone_diff_state = dict(idx_min_dist=idx_min_dist, cr_img_coordinates_sorted=cr_img_coordinates_sorted)
-        return self.backbone_diff_state["idx_min_dist"], self.backbone_diff_state["cr_img_coordinates_sorted"]
-
-    def backbone_diff( self, cr_img_coordinates, img_idx_data ):
-        """
-            Compute the distance of each CR pixel to the closest reconstruction point in image coordinates.
-
-            Arguments
-            ----------
-            cr_img_coordinates : m-by-2 tensor
-                Tensor containing the image coordinates of CR pixels.
-
-            img_idx_data :m-by-1 tensor
-                Tensor containing the index of the image a point was taken from.
-       """
-        curve_pixel_coordinates = self.get_img_coordinates()
-        diffs = None
-        idx_min_dist, cr_img_coordinates_sorted = self.get_backbone_diff_idx(cr_img_coordinates, img_idx_data)
-        for i in np.unique(img_idx_data):
-            diffs = curve_pixel_coordinates[i] - cr_img_coordinates_sorted[i][idx_min_dist[i], :] if diffs is None else torch.concatenate(
-                (diffs, curve_pixel_coordinates[i] - cr_img_coordinates_sorted[i][idx_min_dist[i], :]), 0)
-        return diffs
-
-    def backbone_loss( self, img_coordinates, img_idx_data ):
-        """
-            Computes the average distance of each backbone point to the corresponding CR pixel.
-        """
-        # Penalizes the minimum distance of each measurement point to the reconstructed curve.
-        return torch.linalg.vector_norm(self.backbone_diff(img_coordinates, img_idx_data), self.dist_norm, 1).mean()  # **self.dist_norm
-
-    def loss( self, img_coordinates, img_idx_data ):
-        """
-            Combines the two cost as a weighted sum using w as the weight.
-
-            Arguments
-            ----------
-            img_coordinates : m-by-2 tensor
-                Tensor containing the image coordinates of CR pixels.
-
-            img_idx_data :m-by-1 tensor
-                Tensor containing the index of the image a point was taken from.
-       """
-        loss = 0
-        if self.w < 1.:
-            loss += self.pixel_loss(img_coordinates, img_idx_data) * (1 - self.w)
-        if self.w > 0.:
-            loss += self.backbone_loss(img_coordinates, img_idx_data) * self.w
-        return loss
-
-    def loss_3d_dist( self, s, pts ):
-        """
-            Cost function for a labeled set of 3D points with their corresponding arc-length. The weight w is used to
-            weight the two cost functions, average distance of the backbone points to the 3D points and distance of the
-            tip of the cr to the last 3D point.
-
-            Arguments
-            ----------
-            s : m-by-1 tensor
-                Tensor of (approximated) arc-lengths.
-
-            pts : m-by-3 tensor
-                3D points of the cr that are known.
-        """
-        pt_idc_0 = torch.argmin(torch.abs(self.s_val.reshape(-1, 1) - s.reshape(1, -1)), 0)
-        backbone_pts = self.curve_model(self.s_val)
-        return ((1 - self.w) * torch.linalg.vector_norm(backbone_pts[pt_idc_0, :] - pts, self.dist_norm, 1).mean() + self.w * torch.linalg.vector_norm(
-            pts[-1, :] - pts[-1, :], self.dist_norm, 0))
-
-    def fit( self, pixel_list, optimizer=None, n_iter=5, batch_size=None, lr=0.2, repetitions=1, grad_tol=1e-4, scheduler=None ):
-        """
-            Run the optimization given the the image coordinates of the CR. Per default, an Adam optimizer is used, the full dataset is used and the point correspondances
-            are reset after each gradient descent step.
-
-            Arguments
-            ----------
-            optimizer : PyTorch optimizer
-                Adam with a small weight decay value (1e-6) is recommended.
-
-            pixel_list : list
-                List of pixels corresponding to the CR in each image. The length has to match
-                the number of camera calibration parameters.
-
-            n_iter : int
-                Number of epochs, so how often the data set is used for optimization.
-
-            lr : double
-                Learning rate of the default optimizer.
-
-            batch_size : int
-                Number of CR pixels used per Stochastic Gradient Descent step.
-
-            repetitions : int
-                Number how often the same batch is reused, reducing the need for recalculating the point correspondances.
-
-            grad_tol : double
-                Tolerance on the necessary condition of optimality. If the abolsute value of all partial derivatives is below grad_tol, the algorithm terminates
-                early.
-        """
-        if len(pixel_list) != len(self.camera_calibration_parameters):
-            raise Exception("The list containing the pixel positions of the CR has to match in length the number of given camera calibration parameters.")
-
-        if optimizer is None:
-            optimizer = torch.optim.Adam(self.curve_model.parameters(), lr, weight_decay=1e-6)
-            
-        use_scheduler = scheduler is not None
-
-        dataset = PixelDataset(pixel_list)
-        
-        loss_hist = []
-
-        if batch_size is None:
-            batch_size = int(len(dataset))
-        dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True, num_workers=0, persistent_workers=False)
-        
-        with torch.no_grad():
-            loss_hist.append(self.loss(torch.from_numpy(dataset.p), torch.from_numpy(dataset.img_idx_data)).detach().numpy())
-            lowest_loss = loss_hist[-1]
-            best_model = deepcopy(self.curve_model.state_dict())
-        
-        for i in range(1, n_iter + 1):
-            with tqdm(enumerate(dataloader)) as pbar:
-                for j, (smpl, idc) in pbar:
-                    if smpl.shape[0] < batch_size:
-                        continue
-                    for k in range(repetitions):
-                        optimizer.zero_grad()
-                        self.__bb_pixel_coordinates = None
-                        loss = self.loss(smpl, idc)
-                        loss.backward()
-                        pbar.set_postfix(loss=loss.item(), lr=optimizer.param_groups[0]['lr'])
-                        pbar.set_description(f"Epoch {i}/{n_iter}, Iteration {j + 1}")
-                        optimizer.step()
-                        if use_scheduler:
-                            scheduler.step(loss)
-                        self.curve_model.set_funs()
-                        for f in self.post_step_cb:
-                            f(self)
-                        if ~torch.any(torch.tensor([torch.any(torch.abs(i.grad) >= grad_tol) for i in self.curve_model.parameters()]).bool()):
-                            break
-                    self.reset_diff_states()
-                    for f in self.post_epoch_cb:
-                        f(self)
-            
-            if ~torch.any(torch.tensor([torch.any(torch.abs(i.grad) >= grad_tol) for i in self.curve_model.parameters()]).bool()):
-                break
-            with torch.no_grad():
-                loss_hist.append(self.loss(torch.from_numpy(dataset.p), torch.from_numpy(dataset.img_idx_data)).detach().numpy())
-            if loss_hist[-1] < lowest_loss:
-                best_model = deepcopy(self.curve_model.state_dict())
-                lowest_loss = loss_hist[-1]
-        self.curve_model.load_state_dict(best_model)
-        return loss_hist
+# -*- coding: utf-8 -*-
+"""
+This script contains a PyTorch-based implementation of the continuum robot reconstruction algorithm presented in xxx.
+The package needs a PyTorch build with LAPACK/BLAS, the easiest way for getting this is by installing PyTorch using Conda/Anaconda.
+"""
+
+import torch
+import torch.nn as nn
+import numpy as np
+from .utils import fromWorld2Img, ball_tree_norm, PixelDataset
+from abc import ABC, abstractmethod
+from torchdiffeq import odeint as odeint
+from torch.utils.data import DataLoader
+from tqdm import tqdm
+from warnings import warn
+from copy import deepcopy
+
+
+class TorchParameterizedFunction(nn.Module, ABC):
+    """
+        Class for storing parameterized functions for usage with TorchMovingFrame.
+        Can also be used for other models like polynomials, but it's original purpose was the
+        usage as curvature polynomials.
+    """
+
+    @abstractmethod
+    def get_u_fun( self, idx, s0, s1 ):
+        pass
+
+
+class Polynomial3Torch(TorchParameterizedFunction):
+    r"""
+        Parameterization of degree 3 polynomials. The parameters are the function value and the derivative at start and end.
+        This, for example, allows for easy initialization given simulation results from physics-based models.
+
+        .. note::
+            The parameters for the polynomials are given as
+            :math:`up(i,:) = [f(l[i-1]), f'(l[i-1]), f(l[i]), f'(l[i])]`
+
+        Arguments
+        ----------
+        n : int
+            Number of polynomials used to approximate the cr. Typically set to the number of tubes.
+
+        u_p : str or n-by-4 tensor
+            Optional initialization of the curvature parameters.
+
+        continuous : boolean
+            If True, the polynomials are forced to be continuous.
+
+        random_init : boolean
+            If True and u_p is None, the parameters are initialized randomly.
+
+        end_no_curvature : boolean
+            If True, the last polynomial is forced to be 0. This allows for physically more reasonable uz, so
+            :math:`f_n(s) = 0`
+    """
+
+    def __init__( self, n, u_p=None, optimize=True, continuous=False, random_init=False, end_no_curvature=False ):
+        super().__init__()
+        self.n = n
+        if u_p is not None:
+            _u_p = u_p.clone().detach()
+        if continuous and optimize:
+            n_f = n - end_no_curvature * 2 + 1
+            n_f_dot = n - end_no_curvature
+            if u_p is None:
+                self.u_params = nn.Parameter(10 * (torch.rand(n_f, 1) - 0.5) if random_init else torch.zeros(n_f, 1))
+                self.u_dot_params = nn.Parameter(10 * (torch.rand(n_f_dot, 2) - 0.5) if random_init else torch.zeros(n_f_dot, 2))
+                u_node = torch.concatenate((self.u_params, torch.zeros(2, 1)), 0) if end_no_curvature else self.u_params
+                u_dot_node = torch.concatenate((self.u_dot_params, torch.zeros(1, 2)), 0) if end_no_curvature else self.u_dot_params
+            else:
+                self.u_params = nn.Parameter(torch.cat((_u_p[:, 0, None], _u_p[-1, 2, None, None]), 0))
+                self.u_dot_params = nn.Parameter(_u_p[:, 1::2])
+                u_node = torch.concatenate((self.u_params, torch.zeros(2, 1)), 0) if end_no_curvature else self.u_params
+                u_dot_node = torch.concatenate((self.u_dot_params, torch.zeros(1, 2)), 0) if end_no_curvature else self.u_dot_params
+            self.u_p = torch.concatenate((u_node[:-1, :], u_dot_node[:, 0, None], u_node[1:, :], u_dot_node[:, 1, None]), 1)
+        else:
+            if u_p is None and optimize:
+                self.u_p = nn.Parameter(10 * (torch.rand(n, 4) - 0.5) if random_init else torch.zeros(n, 4))
+            elif u_p is None and not optimize:
+                self.register_buffer('u_p', torch.zeros(n, 4))
+            elif optimize:
+                self.u_p = nn.Parameter(_u_p)
+            else:
+                self.register_buffer('u_p', _u_p)
+
+    def get_u_fun( self, idx, s0, s1 ):
+        r"""
+            Function for generating the degree 3 polynomial from the curvature parameters.
+            u_p = [f(s0), f'(s0), f(s1), f'(s1)]
+        """
+        u_p = self.u_p[idx, :]
+        T = s1 - s0
+        a = (2 * u_p[0] - 2 * u_p[2] + T * u_p[1] + T * u_p[3]) / (T ** 3)
+        b = -(3 * u_p[0] - 3 * u_p[2] + 2 * T * u_p[1] + T * u_p[3]) / (T ** 2)
+        c = u_p[1]
+        d = u_p[0]
+
+        def u_fun( s ):
+            return torch.stack([d, c, b, a]) @ ((s - s0) ** (torch.arange(0, 4)).reshape(4, 1))
+
+        return u_fun
+
+
+class PolynomialKTorch(TorchParameterizedFunction):
+    r"""
+        Parameterization of degree K polynomials for the curvatures used by TorchMovingFrame.
+
+        Arguments
+        ----------
+        n : int
+            Number of polynomials used to approximate the cr. Typically set to the number of tubes.
+
+        K : int
+            Degree used for the polynomials.
+
+        u_p : str or n-by-K tensor
+            Optional initialization of the curvature parameters.
+
+        optimize : boolean
+            If True, the parameters are optimized during the fitting process.
+
+        random_init : boolean
+            If True and u_p is None, the parameters are initialized randomly.
+
+        end_no_curvature : boolean
+            If True, the last polynomial is forced to be 0. This allows for physically more reasonable uz, so
+    """
+
+    def __init__( self, n, K, u_p=None, optimize=True, random_init=False, end_no_curvature=False ):
+        super().__init__()
+        self.n = n
+        self.K = K
+        if u_p is not None:
+            _u_p = u_p.clone().detach()
+        if optimize:
+            n_f = n - end_no_curvature
+            if u_p is None:
+                self.u_params = nn.Parameter(10 * (torch.rand(n_f, K + 1) - 0.5) if random_init else torch.zeros(n_f, K + 1))
+            else:
+                self.u_params = nn.Parameter(_u_p[:n_f, :])
+            self.u_p = torch.concatenate((self.u_params, torch.zeros(1, K + 1)), 0) if end_no_curvature else self.u_params
+        else:
+            if u_p is None:
+                self.register_buffer('u_p', torch.zeros(n, K + 1))
+            else:
+                self.register_buffer('u_p', _u_p)
+
+    def get_u_fun( self, idx, s0, s1 ):
+        '''
+            Function for generating the K-th-ordner polynomial from the curvature parameters.
+        '''
+
+        def u_fun( s ):
+            return self.u_p[idx, :] @ (((s - s0)/(s1 - s0)) ** (torch.arange(0, self.K + 1)).reshape(self.K + 1, 1))
+
+        return u_fun
+
+def __curvature_matrix_rotm( ux, uy, uz ):
+    null = torch.zeros([1])
+    elems = [[null, null, uy], [uz, null, null], [null, ux, null]]
+    curvature_mat = torch.stack([torch.concatenate(i, 0) for i in elems], 0)
+    return curvature_mat - curvature_mat.T
+
+def __curvature_matrix_quat( ux, uy, uz ):
+    null = torch.zeros([1])
+    elems = [[null, null, null, null], [ux, null, uz, null], [uy, null, null, ux],[uz, uy, null, null]]
+    curvature_mat = torch.stack([torch.concatenate(i, 0) for i in elems], 0)
+    return curvature_mat - curvature_mat.T
+
+CURVATURE_FCN = {'rotm':__curvature_matrix_rotm, 'quat':__curvature_matrix_quat}
+
+class TorchPolynomialCurve(nn.Module):
+    """
+        NOTE: It is not recommended to use this class. It was developed for research purposes, so it is kept for reference.
+        This class implements the a direct polynomial formulation for reconstructing a continuum robot's backbone.
+        The parameterization of the curvatures ux, uy, and uz is achieved by providing TorchParameterizedFunction objects.
+
+        Arguments
+        ----------
+        l : tensor
+            List of the lengths up to which the corresponding polynomial is used. Is
+            typically selected to be each NiTi tube's length outside of the actuation
+            unit.
+
+        p0 : 3-by-1 tensor
+            A 3D point where the CR exits the actuation unit in world
+            coordinates.
+
+        p0_parametric : boolean
+            If True, the initial position p0 is estimated as well.
+
+        ux : n-by-4 tensor or TorchParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the x-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        uy : n-by-4 tensor or TorchParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the y-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        uz : n-by-4 tensor or TorchParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the z-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        optimize : list of 3 booleans
+            If True, the corresponding curvature [ ux, uy, uz ] is optimized during the fitting process. Only used if the 
+            corresponding curvature is not given as a TorchParameterizedFunction object.
+
+        continuous_u : list of 3 booleans
+            If true, the corresponding curvature [ ux, uy, uz ] is enforced to be continuous. Only used if the 
+            corresponding curvature is not given as a TorchParameterizedFunction object.
+
+        random_init : list of 3 booleans
+            If true, the corresponding curvature [ ux, uy, uz ] is randomly initialized. Only used if the 
+            corresponding curvature is not given as a TorchParameterizedFunction object.
+
+    """
+    
+    def __init__(
+            self, l, p0=torch.zeros(3, 1), p0_parametric=False, 
+            ux=None, uy=None, uz=None, optimize=[True, True, True], continuous_u=[True, True, True], 
+            random_init=[False] * 3 
+            ):
+        super().__init__()
+        
+        self.ux_funs, self.uy_funs, self.uz_funs = None, None, None
+
+        self.l = l
+        self.n = len(l)
+        
+        if p0_parametric:
+            self.p0 = nn.Parameter(p0)
+        else:
+            self.p0 = p0
+            
+        if issubclass(type(ux), TorchParameterizedFunction):  # Check if ux is already a TorchParameterizedFunction.
+            self.ux = ux
+        else:  # If not, initialize it as a Polynomial3Torch.
+            self.ux = Polynomial3Torch(self.n, ux, optimize=optimize[0], continuous=continuous_u[0], random_init=random_init[0])
+
+        if issubclass(type(uy), TorchParameterizedFunction):  # Check if uy is already a TorchParameterizedFunction.
+            self.uy = uy
+        else:  # If not, initialize it as a Polynomial3Torch.
+            self.uy = Polynomial3Torch(self.n, uy, optimize=optimize[1], continuous=continuous_u[1], random_init=random_init[1])
+
+        if issubclass(type(uz), TorchParameterizedFunction):  # Check if uz is already a TorchParameterizedFunction.
+            self.uz = uz
+        else:  # If not, initialize it as a Polynomial3Torch.
+            self.uz = Polynomial3Torch(self.n, uz, optimize=optimize[2], continuous=continuous_u[2], random_init=random_init[2])
+
+        self.set_funs()
+        
+    def set_funs( self ):
+        """
+            Function that fills the curvature function handles. Has to be called after each optimizer step.
+        """
+        self.ux_funs = [self.ux.get_u_fun(0, 0, self.l[0])]
+        self.uy_funs = [self.uy.get_u_fun(0, 0, self.l[0])]
+        self.uz_funs = [self.uz.get_u_fun(0, 0, self.l[0])]
+
+        for i in range(1, self.n):
+            self.ux_funs.append(self.ux.get_u_fun(i, self.l[i - 1], self.l[i]))
+            self.uy_funs.append(self.uy.get_u_fun(i, self.l[i - 1], self.l[i]))
+            self.uz_funs.append(self.uz.get_u_fun(i, self.l[i - 1], self.l[i]))
+            
+    def forward( self, s_val ):
+        """
+        TODO: Something about this is off, but I cannot figure out what it is.
+        """
+        for i in range(len(self.l)):
+            s = s_val[(s_val <= self.l[i]) & ((self.l[i-1] if i >= 1 else 0) <= s_val)]
+            if i == 0:
+                p = torch.stack([self.ux_funs[i](s), self.uy_funs[i](s), self.uz_funs[i](s)], 0)
+            else:
+                p = torch.stack([self.ux_funs[i](s), self.uy_funs[i](s), self.uz_funs[i](s)], 0)
+        
+        return p.T
+
+
+class TorchMovingFrame(nn.Module):
+    """
+        This class implements the moving frame formulation for reconstructing a continuum robot's backbone.
+        The parameterization of the curvatures ux, uy, and uz is achieved by providing TorchParameterizedFunction objects.
+
+        Arguments
+        ----------
+        l : tensor
+            List of the lengths up to which the corresponding polynomial is used. Is
+            typically selected to be each NiTi tube's length outside of the actuation
+            unit.
+
+        p0 : 3-by-1 tensor
+            A 3D point where the CR exits the actuation unit in world
+            coordinates.
+
+        p0_parametric : boolean
+            If True, the initial position p0 is estimated as well.
+
+        R0 : 3-by-3 or 4-by-1 tensor
+            Either a 3-by-3 matrix from SO(3) that describes the orientation of
+            the exiting CR (ref. [1]) or, if R0_parametric is True, tensor of
+            shape (4,). The matrix is then parametrized using quaternions.
+
+        R0_parametric : boolean
+            If True, the initial orientation R0 is estimated as well. To ensure
+            that R0 remains inside SO(3), it is parameterized using quaternions.
+
+        ux : n-by-4 tensor or TorchParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the x-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        uy : n-by-4 tensor or TorchParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the y-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        uz : n-by-4 tensor or TorchParameterizedFunction
+            Initial guess for the parameters of the polynomials
+            for the z-curvatures of the n polynomials. If set to None it is either initialized
+            as 0s or uniformly distributed between -5 and 5 if random_init is True.
+
+        optimize : list of 3 booleans
+            If True, the corresponding curvature [ ux, uy, uz ] is optimized during the fitting process. Only used if the 
+            corresponding curvature is not given as a TorchParameterizedFunction object.
+
+        integrator : str
+            Integration method from the following list:
+
+                - "midpoint"
+                - "rk4"
+                - "dopri5",
+                - "bost3"
+                - "fehlberg2"
+                - "adaptive_heun"
+                - "euler"
+                - "dopri8"
+                - "explicit_adams"
+                - "implicit_adams"
+
+            The midpoint rule typically gives a good trade-off between accuracy and speed.
+
+        continuous_u : list of 3 booleans
+            If true, the corresponding curvature [ ux, uy, uz ] is enforced to be continuous. Only used if the 
+            corresponding curvature is not given as a TorchParameterizedFunction object.
+
+        random_init : list of 3 booleans
+            If true, the corresponding curvature [ ux, uy, uz ] is randomly initialized. Only used if the 
+            corresponding curvature is not given as a TorchParameterizedFunction object.
+
+        Sources
+        ----------
+        [1] 10.1109/TRO.2010.2062570, Rucker, D. Caleb, Bryan A. Jones, and Robert J. Webster III. "A geometrically exact model for externally loaded concentric-tube continuum robots." IEEE transactions on robotics 26.5 (2010): 769-780.
+    """
+
+    def __init__(
+            self, l, p0=torch.zeros(3, 1), p0_parametric=False, R0=None, R0_parametric=False, rotation_method="rotm", 
+            ux=None, uy=None, uz=None, optimize=[True, True, False], integrator='midpoint', continuous_u=[False, False, True], 
+            random_init=[False] * 3 
+            ):
+        super().__init__()
+
+        self.__integrator = 'midpoint'
+        self.__previous_integrate_parameters = None
+        self.ux_funs, self.uy_funs, self.uz_funs = None, None, None
+        self.rotation_method = rotation_method
+
+        self.l = l
+        self.n = len(l)
+
+        if p0_parametric:
+            self.p0 = nn.Parameter(p0)
+        else:
+            self.p0 = p0
+        
+        if R0 is None:
+            if rotation_method == "quat" or R0_parametric:
+                R0 = torch.tensor([1, 0, 0, 0])
+            else:
+                R0 = torch.eye(3)
+        
+        if R0_parametric:
+            # If R0 is parametric, it is assumed to be a quaternion. The quaternion is then normalized and converted to a rotation matrix.
+            if R0.shape != torch.Size([4, ]):
+                raise Exception("If R0_parametric is set to true, the input R0 is considered to be a quaternion, so its shape is supposed to be (4,).")
+            _R0 = R0.float()
+            self.q = nn.Parameter(_R0 / torch.linalg.vector_norm(_R0))
+            q = self.q / torch.linalg.vector_norm(self.q)  # Setup the quaternion.
+            
+            if rotation_method == "quat":
+                self.R0 = q
+            else:
+                self.R0 = torch.zeros((3, 3))
+                # Convert the quaternion to a rotation matrix R0.
+                self.R0[0, 0] = 1 - 2 * (q[2] ** 2 + q[3] ** 2)
+                self.R0[0, 1] = 2 * (q[1] * q[2] - q[0] * q[3])
+                self.R0[0, 2] = 2 * (q[1] * q[3] + q[0] * q[2])
+                self.R0[1, 0] = 2 * (q[1] * q[2] + q[0] * q[3])
+                self.R0[1, 1] = 1 - 2 * (q[1] ** 2 + q[3] ** 2)
+                self.R0[1, 2] = 2 * (q[2] * q[3] - q[0] * q[1])
+                self.R0[2, 0] = 2 * (q[1] * q[3] - q[0] * q[2])
+                self.R0[2, 1] = 2 * (q[2] * q[3] + q[0] * q[1])
+                self.R0[2, 2] = 1 - 2 * (q[1] ** 2 + q[2] ** 2)
+        else:
+            self.R0 = R0
+        
+        self.x0 = torch.cat((self.p0.flatten(), self.R0.flatten()), 0)
+        self.integrator = integrator
+        self.ode_solution = None
+        self.ode = self.__quat_ode if rotation_method == "quat" else self.__rotm_ode
+        self.curvature_mat_fcn = CURVATURE_FCN[rotation_method]
+
+        if issubclass(type(ux), TorchParameterizedFunction):  # Check if ux is already a TorchParameterizedFunction.
+            self.ux = ux
+        else:  # If not, initialize it as a Polynomial3Torch.
+            self.ux = Polynomial3Torch(self.n, ux, optimize=optimize[0], continuous=continuous_u[0], random_init=random_init[0])
+
+        if issubclass(type(uy), TorchParameterizedFunction):  # Check if uy is already a TorchParameterizedFunction.
+            self.uy = uy
+        else:  # If not, initialize it as a Polynomial3Torch.
+            self.uy = Polynomial3Torch(self.n, uy, optimize=optimize[1], continuous=continuous_u[1], random_init=random_init[1])
+
+        if issubclass(type(uz), TorchParameterizedFunction):  # Check if uz is already a TorchParameterizedFunction.
+            self.uz = uz
+        else:  # If not, initialize it as a Polynomial3Torch.
+            self.uz = Polynomial3Torch(self.n, uz, optimize=optimize[2], continuous=continuous_u[2], random_init=random_init[2])
+
+        self.set_funs()  # Fill the curvature function handles.
+
+    def set_funs( self ):
+        """
+            Function that fills the curvature function handles. Has to be called after each optimizer step.
+        """
+        self.ux_funs = [self.ux.get_u_fun(0, 0, self.l[0])]
+        self.uy_funs = [self.uy.get_u_fun(0, 0, self.l[0])]
+        self.uz_funs = [self.uz.get_u_fun(0, 0, self.l[0])]
+
+        for i in range(1, self.n):
+            self.ux_funs.append(self.ux.get_u_fun(i, self.l[i - 1], self.l[i]))
+            self.uy_funs.append(self.uy.get_u_fun(i, self.l[i - 1], self.l[i]))
+            self.uz_funs.append(self.uz.get_u_fun(i, self.l[i - 1], self.l[i]))
+
+    @property
+    def integrator( self ):
+        return self.__integrator
+
+    @integrator.setter
+    def integrator( self, value ):
+        if value not in ["midpoint", "rk4", "dopri5", "bosh3", "fehlberg2", "adaptive_heun", "euler", "dopri8", "explicit_adams", "implicit_adams"]:
+            raise Exception(
+                "The given integrator is not valid or available. Please use one of the solvers given by the torchdiffeq package: https://github.com/rtqichen/torchdiffeq")
+        if value != self.__integrator:
+            """
+                Ensure that the integration is run again after the integrator was changed.
+            """
+            self.__previous_integrate_parameters = None
+        self.__integrator = value
+
+    def u_hat( self, s ):
+        """
+            Function for transforming u_p to the necessary skew-symmstric matrix. idx_fun is the index of the curvature function that is active at the current
+            arc-length.
+        """
+        if s <= self.l[-1]:
+            active_tube_idx = torch.where(self.l >= s)[0]
+            idx_fun = torch.min(active_tube_idx)
+        else:
+            idx_fun = self.n - 1
+
+        ux, uy, uz = self.ux_funs[idx_fun](s), self.uy_funs[idx_fun](s), self.uz_funs[idx_fun](s)
+        curvature_mat = self.curvature_mat_fcn( ux, uy, uz )
+        return curvature_mat
+    
+    def forward( self, s_val ):
+        return self.integrate(s_val)[:,:3]
+    
+    def integrate( self, s_val ):
+        """
+            Get the solution of the integration. Integration is only performed if the previous (curvature) parameters did change or if
+            the integration scheme changed.
+
+            Arguments:
+            ----------
+            s_val : tensor, optional
+                If values for the arc-length are given, the integration scheme is evaluated at these points and not the
+                ones used in the integration. This is useful for plotting the solution. If None, the arc-lengths used in the integration.
+        """
+        if self.__previous_integrate_parameters is None or (list(self.__previous_integrate_parameters()) == list(self.parameters())):            
+            self.ode_solution = odeint(self.ode, self.x0, s_val, method=self.integrator)
+        return self.ode_solution
+       
+    def __quat_ode( self, s, x ):
+        """
+            Right-hand side of the quaternion moving frame ODE.
+
+            Arguments
+            ----------
+            s : float
+                The current value of the arc-length.
+
+            x : 7-by-1 float tensor
+                The current state x = [p, q]. p is the position of the CR in world coordinates and q is the quaternion describing the orientation of the
+                CR at the current arc-length.
+        """
+        q = x[3:]
+        dp1 = (q[1]*q[3]+q[0]*q[2])
+        dp2 = (q[2]*q[3]-q[0]*q[1])
+        dp3 = (-q[1]**2-q[2]**2)
+        dp = torch.tensor([0,0,1])+2*torch.stack([dp1, dp2, dp3])/(torch.sum(q**2))
+        dq = self.u_hat(s)@q/2
+        return torch.concat((dp, dq), 0)
+    
+    def __rotm_ode( self, s, x ):
+        """
+            Right-hand side of the moving frame ODE.
+
+            Arguments
+            ----------
+            s : float
+                The current value of the arc-length.
+
+            x : 12-by-1 float tensor
+                The current state x = [p, R]. p is the position of the CR in world coordinates and R is the rotation matrix describing the orientation of the
+                CR at the current arc-length.
+        """
+        R = x[3:].reshape((3, 3))
+
+        dp = R[:, 2].flatten()
+        dR = (R @ self.u_hat(s)).flatten()
+        return torch.concat((dp, dR), 0)
+    
+
+class TorchCurveEstimator():
+    r"""
+        This class implements the PyTorch-based curve estimator (TCE) for continuum robots.
+        The TCE takes a parameterized model for the continuum robot - this can be a rotation
+        frame, circular arcs, differentiable rendering model, ... - and optimizes for the
+        torch.parameters using an Iterative Closest Point algorithm.
+
+        Arguments
+        ----------
+        curve_model : nn.Module
+            PyTorch model that parameterizes the reconstruction of thecontinuum robot. The model has to be
+            callable with the arc-length as the only argument.
+        
+        l : positive scalar
+            The length of the continuum robot from the starting position to the tip of the robot.
+
+        camera_calibration_parameters : list of dictionaries
+            A list of dictionaries containing the keys
+            "A", "dist", "P", "R", and "T". The function "camera_folder_to_params" can
+            automatically generate this list for you.
+
+        n_steps : int
+            Number of intermediate steps to evaluate the reconstructed cr at.
+            If low, the computation is fast, but for very low values the convergence might
+            be bad. If high, a better solution might be found, at cost of higher computation
+            times.
+
+        w : double
+            Weighting of the two cost functions. 0 (only track distance of pixels to
+            reconstruction) is typically a good value, but if parts of the cr are occluded,
+            increasing w can help.
+
+        dist_norm : int
+            Order of the metric used to penalize distances. Higher values give more cost to big errors.
+    """
+    
+    def __init__(self, curve_model, camera_calibration_parameters, l, w=0., n_steps=50, dist_norm=2, post_step_cb=[], post_epoch_cb=[] ):
+        super().__init__()
+        assert isinstance(curve_model, nn.Module), "The curve_model needs to be an instance of nn.Module" 
+        self.camera_calibration_parameters = camera_calibration_parameters
+        self.curve_model = curve_model
+        self.l = l
+        
+        self.w = w
+        self.n_steps = n_steps
+        self.dist_norm = dist_norm
+        self.pixel_diff_state = None
+        self.backbone_diff_state = None
+        self.__bb_pixel_coordinates = None
+        if len(camera_calibration_parameters) < 2:
+            warn("Two or more images are necessary for a successful reconstruction.")
+        self.camera_calibration_parameters = camera_calibration_parameters
+        self.s_val = torch.linspace(0, self.l, self.n_steps)
+        self.reset_diff_states()
+        self.post_step_cb = post_step_cb
+        self.post_epoch_cb = post_epoch_cb
+
+    def get_img_coordinates( self ):
+        """
+            Project the computed backbone points to all the images and return the image coordinates.
+        """
+        if self.__bb_pixel_coordinates is None:
+            backbone_pts = self.curve_model(self.s_val).T
+            self.__bb_pixel_coordinates = []
+            for i in range(len(self.camera_calibration_parameters)):
+                self.__bb_pixel_coordinates.append(fromWorld2Img(backbone_pts, **self.camera_calibration_parameters[i]).T)
+        return self.__bb_pixel_coordinates
+
+    def reset_diff_states( self ):
+        """
+            Reset the diff states, so that in the next call off get_*_diff_idx, the correspondances are computated agian.
+        """
+        self.pixel_diff_state = None
+        self.backbone_diff_state = None
+
+    def get_pixel_diff_idx( self, cr_img_coordinates, img_idx_data ):
+        """
+            Computes for each CR pixel the index of the closest reconstruction pixel.
+
+            Arguments
+            ----------
+            cr_img_coordinates : m-by-2 int
+                Coordinates of CR pixels in image coordinates.
+
+            img_idx_data : m-by-1 int
+                Vector containing the index from which image the corresponding img_coordinates entry was taken.
+        """
+        backbone_img_coordinates = self.get_img_coordinates()
+        if self.pixel_diff_state is None:
+            idx_min_dist = []
+            cr_img_coordinates_sorted = []
+            for i in np.unique(np.unique(img_idx_data)):
+                cr_img_coordinates_i = cr_img_coordinates[img_idx_data == i, :]
+                # _, idc_min = brute_force_distance_norm(cr_img_coordinates_i.float(), backbone_img_coordinates[i], p=self.dist_norm)
+                idc_min = ball_tree_norm(cr_img_coordinates_i.float(), backbone_img_coordinates[i], p=self.dist_norm)
+                idx_min_dist.append(idc_min)
+                cr_img_coordinates_sorted.append(cr_img_coordinates_i)
+            self.pixel_diff_state = dict(idx_min_dist=idx_min_dist, cr_img_coordinates_sorted=cr_img_coordinates_sorted)
+        
+        return self.pixel_diff_state["idx_min_dist"], self.pixel_diff_state["cr_img_coordinates_sorted"]
+
+    def pixel_diff( self, cr_img_coordinates, img_idx_data ):
+        """
+            Compute the distance of each CR pixel to the closest reconstruction point in image coordinates.
+
+            Arguments
+            ----------
+            cr_img_coordinates : m-by-2 tensor
+                Tensor containing the image coordinates of CR pixels.
+
+            img_idx_data :m-by-1 tensor
+                Tensor containing the index of the image a point was taken from.
+       """
+        curve_pixel_coordinates = self.get_img_coordinates()
+        diffs = None
+        idx_min_dist, cr_img_coordinates_sorted = self.get_pixel_diff_idx(cr_img_coordinates, img_idx_data)
+        for i in np.unique(img_idx_data):
+            diffs = curve_pixel_coordinates[i][idx_min_dist[i], :] - cr_img_coordinates_sorted[i] if diffs is None else torch.concatenate(
+                (diffs, curve_pixel_coordinates[i][idx_min_dist[i], :] - cr_img_coordinates_sorted[i]), 0)
+        return diffs
+
+    def pixel_loss( self, cr_img_coordinates, img_idx_data ):
+        """
+            Computes the average distance of each CR pixel to the corresponding backbone point.
+        """
+        # Penalizes the minimum distance of each measurement point to the reconstructed curve.
+        return torch.linalg.vector_norm(self.pixel_diff(cr_img_coordinates, img_idx_data), self.dist_norm, 1).mean()  # **self.dist_norm
+
+    def get_backbone_diff_idx( self, cr_img_coordinates, img_idx_data ):
+        """
+            Computes for each backbone point in image coordinates the index of the closest CR pixel .
+
+            Arguments
+            ----------
+            cr_img_coordinates : m-by-2 int
+                Coordinates of CR pixels in image coordinates.
+
+            img_idx_data : m-by-1 int
+                Vector containing the index from which image the corresponding img_coordinates entry was taken.
+
+        """
+        backbone_img_coordinates = self.get_img_coordinates()
+        if self.backbone_diff_state is None:
+            idx_min_dist = []
+            cr_img_coordinates_sorted = []
+            for i in np.unique(np.unique(img_idx_data)):
+                cr_img_coordinates_i = cr_img_coordinates[img_idx_data == i, :]
+                # _, idc_min = brute_force_distance_norm(backbone_img_coordinates[i], cr_img_coordinates_i.float(), p=self.dist_norm)
+                idc_min = ball_tree_norm(backbone_img_coordinates[i], cr_img_coordinates_i.float(), p=self.dist_norm)
+                idx_min_dist.append(idc_min)
+                cr_img_coordinates_sorted.append(cr_img_coordinates_i)
+            self.backbone_diff_state = dict(idx_min_dist=idx_min_dist, cr_img_coordinates_sorted=cr_img_coordinates_sorted)
+        return self.backbone_diff_state["idx_min_dist"], self.backbone_diff_state["cr_img_coordinates_sorted"]
+
+    def backbone_diff( self, cr_img_coordinates, img_idx_data ):
+        """
+            Compute the distance of each CR pixel to the closest reconstruction point in image coordinates.
+
+            Arguments
+            ----------
+            cr_img_coordinates : m-by-2 tensor
+                Tensor containing the image coordinates of CR pixels.
+
+            img_idx_data :m-by-1 tensor
+                Tensor containing the index of the image a point was taken from.
+       """
+        curve_pixel_coordinates = self.get_img_coordinates()
+        diffs = None
+        idx_min_dist, cr_img_coordinates_sorted = self.get_backbone_diff_idx(cr_img_coordinates, img_idx_data)
+        for i in np.unique(img_idx_data):
+            diffs = curve_pixel_coordinates[i] - cr_img_coordinates_sorted[i][idx_min_dist[i], :] if diffs is None else torch.concatenate(
+                (diffs, curve_pixel_coordinates[i] - cr_img_coordinates_sorted[i][idx_min_dist[i], :]), 0)
+        return diffs
+
+    def backbone_loss( self, img_coordinates, img_idx_data ):
+        """
+            Computes the average distance of each backbone point to the corresponding CR pixel.
+        """
+        # Penalizes the minimum distance of each measurement point to the reconstructed curve.
+        return torch.linalg.vector_norm(self.backbone_diff(img_coordinates, img_idx_data), self.dist_norm, 1).mean()  # **self.dist_norm
+
+    def loss( self, img_coordinates, img_idx_data ):
+        """
+            Combines the two cost as a weighted sum using w as the weight.
+
+            Arguments
+            ----------
+            img_coordinates : m-by-2 tensor
+                Tensor containing the image coordinates of CR pixels.
+
+            img_idx_data :m-by-1 tensor
+                Tensor containing the index of the image a point was taken from.
+       """
+        loss = 0
+        if self.w < 1.:
+            loss += self.pixel_loss(img_coordinates, img_idx_data) * (1 - self.w)
+        if self.w > 0.:
+            loss += self.backbone_loss(img_coordinates, img_idx_data) * self.w
+        return loss
+
+    def loss_3d_dist( self, s, pts ):
+        """
+            Cost function for a labeled set of 3D points with their corresponding arc-length. The weight w is used to
+            weight the two cost functions, average distance of the backbone points to the 3D points and distance of the
+            tip of the cr to the last 3D point.
+
+            Arguments
+            ----------
+            s : m-by-1 tensor
+                Tensor of (approximated) arc-lengths.
+
+            pts : m-by-3 tensor
+                3D points of the cr that are known.
+        """
+        pt_idc_0 = torch.argmin(torch.abs(self.s_val.reshape(-1, 1) - s.reshape(1, -1)), 0)
+        backbone_pts = self.curve_model(self.s_val)
+        return ((1 - self.w) * torch.linalg.vector_norm(backbone_pts[pt_idc_0, :] - pts, self.dist_norm, 1).mean() + self.w * torch.linalg.vector_norm(
+            pts[-1, :] - pts[-1, :], self.dist_norm, 0))
+
+    def fit( self, pixel_list, optimizer=None, n_iter=5, batch_size=None, lr=0.2, repetitions=1, grad_tol=1e-4, scheduler=None ):
+        """
+            Run the optimization given the the image coordinates of the CR. Per default, an Adam optimizer is used, the full dataset is used and the point correspondances
+            are reset after each gradient descent step.
+
+            Arguments
+            ----------
+            optimizer : PyTorch optimizer
+                Adam with a small weight decay value (1e-6) is recommended.
+
+            pixel_list : list
+                List of pixels corresponding to the CR in each image. The length has to match
+                the number of camera calibration parameters.
+
+            n_iter : int
+                Number of epochs, so how often the data set is used for optimization.
+
+            lr : double
+                Learning rate of the default optimizer.
+
+            batch_size : int
+                Number of CR pixels used per Stochastic Gradient Descent step.
+
+            repetitions : int
+                Number how often the same batch is reused, reducing the need for recalculating the point correspondances.
+
+            grad_tol : double
+                Tolerance on the necessary condition of optimality. If the abolsute value of all partial derivatives is below grad_tol, the algorithm terminates
+                early.
+        """
+        if len(pixel_list) != len(self.camera_calibration_parameters):
+            raise Exception("The list containing the pixel positions of the CR has to match in length the number of given camera calibration parameters.")
+
+        if optimizer is None:
+            optimizer = torch.optim.Adam(self.curve_model.parameters(), lr, weight_decay=1e-6)
+            
+        use_scheduler = scheduler is not None
+
+        dataset = PixelDataset(pixel_list)
+        
+        loss_hist = []
+
+        if batch_size is None:
+            batch_size = int(len(dataset))
+        dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=True, num_workers=0, persistent_workers=False)
+        
+        with torch.no_grad():
+            loss_hist.append(self.loss(torch.from_numpy(dataset.p), torch.from_numpy(dataset.img_idx_data)).detach().numpy())
+            lowest_loss = loss_hist[-1]
+            best_model = deepcopy(self.curve_model.state_dict())
+        
+        for i in range(1, n_iter + 1):
+            with tqdm(enumerate(dataloader)) as pbar:
+                for j, (smpl, idc) in pbar:
+                    if smpl.shape[0] < batch_size:
+                        continue
+                    for k in range(repetitions):
+                        optimizer.zero_grad()
+                        self.__bb_pixel_coordinates = None
+                        loss = self.loss(smpl, idc)
+                        loss.backward()
+                        pbar.set_postfix(loss=loss.item(), lr=optimizer.param_groups[0]['lr'])
+                        pbar.set_description(f"Epoch {i}/{n_iter}, Iteration {j + 1}")
+                        optimizer.step()
+                        if use_scheduler:
+                            scheduler.step(loss)
+                        self.curve_model.set_funs()
+                        for f in self.post_step_cb:
+                            f(self)
+                        if ~torch.any(torch.tensor([torch.any(torch.abs(i.grad) >= grad_tol) for i in self.curve_model.parameters()]).bool()):
+                            break
+                    self.reset_diff_states()
+                    for f in self.post_epoch_cb:
+                        f(self)
+            
+            if ~torch.any(torch.tensor([torch.any(torch.abs(i.grad) >= grad_tol) for i in self.curve_model.parameters()]).bool()):
+                break
+            with torch.no_grad():
+                loss_hist.append(self.loss(torch.from_numpy(dataset.p), torch.from_numpy(dataset.img_idx_data)).detach().numpy())
+            if loss_hist[-1] < lowest_loss:
+                best_model = deepcopy(self.curve_model.state_dict())
+                lowest_loss = loss_hist[-1]
+        self.curve_model.load_state_dict(best_model)
+        return loss_hist
```

### Comparing `icpReconstructor-0.1.0/icpReconstructor/utils.py` & `icpReconstructor-0.1.1/icpReconstructor/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,693 +1,692 @@
-import casadi
-import numpy as np
-import torch
-import networkx as nx
-from copy import copy
-from sklearn.neighbors import BallTree
-from torch.utils.data import Dataset
-from os.path import sep
-from skimage.morphology import skeletonize_3d
-
-def image_to_idx( img ):
-    """
-        Transform the binary image (img) to coordinates.
-    """
-    im_idc = np.where(img.T)
-    return np.stack(im_idc, 1)
-
-
-def camera_folder_to_params( camera_folder, cams, package="torch" ):
-    """
-        Read the parameters from a folder using predefined file names.
-
-        Arguments
-        ----------
-        camera_folder : str
-            Folder containing the parameter files.
-
-        cams : int or list
-            Either the number of cameras to be used or a list of camera indices.
-    """
-    i_cams = cams if type(cams) is list else list(range(cams))
-
-    param_list = []
-    path = camera_folder if camera_folder[-1] == sep else camera_folder + sep
-    load_and_tensor = {"torch":lambda x: torch.from_numpy(np.load(path + x)).float(), "casadi":lambda x: np.load(path + x)}[package]
-    for i in i_cams:
-        param_list.append({
-            "A": load_and_tensor(f"calib_A{i}.npy"),
-            "dist": load_and_tensor(f"calib_dist{i}.npy"),
-            "P": load_and_tensor(f"calib_P{i}_.npy"),
-            "R": load_and_tensor("cs_conversion_R.npy"),
-            "T": load_and_tensor("cs_conversion_T.npy")})
-    return param_list
-
-
-class PixelDataset(Dataset):
-    """
-        Dataset of all the pixel positions that correspond to the CR.
-
-        Arguments
-        ----------
-            p_list : list
-                List containing the pixel positions.
-
-        Returns
-        ----------
-            p : m-by-2 tensor
-                Tensor of pixel positions.
-
-            img_idx_data : m-by-1 tensor
-                Tensor containing the index of the corresponding camera.
-    """
-
-    def __init__( self, p_list ):
-        self.p = None
-        self.img_idx_data = None
-        for i in range(len(p_list)):
-            p = p_list[i]
-            self.p = p if self.p is None else np.concatenate((self.p, p), 0)
-            self.img_idx_data = i * np.ones((p.shape[0],), dtype=np.int8) if self.img_idx_data is None else np.concatenate(
-                (self.img_idx_data, i * np.ones((p.shape[0],), dtype=np.int8)), 0)
-
-    def __len__( self ):
-        return self.p.shape[0]
-
-    def __getitem__( self, idx ):
-        return (self.p[idx, :], self.img_idx_data[idx])
-
-def brute_force_distance_norm(A, B, p):
-    # Calculate distances using the p-norm
-    distances = torch.cdist(A, B, p=p)**p
-    # Find the index of the nearest point for each point in A
-    return distances, torch.argmin(distances, dim=1)
-
-def ball_tree_norm(A, B, p):
-    r"""
-        Efficiently finds the nearest neighbors from one set of points in A to another set in B using the Minkowski distance metric
-        parameterized by p. The function leverages a Ball Tree structure for fast nearest neighbor searches in high-dimensional spaces.
-    
-        The function converts PyTorch tensors to NumPy arrays, uses the BallTree implementation from sklearn for querying the nearest
-        neighbor, and finally converts the results back to a PyTorch tensor.
-    
-        Arguments
-        ----------
-        A : torch.Tensor
-            A tensor of points for which nearest neighbors in B need to be found. Each row corresponds to a different point.
-    
-        B : torch.Tensor
-            A tensor of points constituting the search space for nearest neighbors. Each row corresponds to a different point.
-    
-        p : int
-            The order of the Minkowski metric to be used for calculating distances. For example, p=2 corresponds to the Euclidean distance.
-    
-        Returns
-        -------
-        torch.Tensor
-            A tensor containing the indices of the nearest neighbors in B for each point in A. The indices are 1-dimensional (flattened).
-    
-        Example
-        -------
-        Suppose you have two sets of points, `points_a` and `points_b`, represented as PyTorch tensors:
-            points_a = torch.tensor([[1.0, 2.0], [2.0, 3.0]])
-            points_b = torch.tensor([[2.0, 1.0], [3.0, 2.0], [1.0, 2.0]])
-    
-        To find the nearest neighbor in `points_b` for each point in `points_a` using the Euclidean distance:
-            nearest_indices = ball_tree_norm(points_a, points_b, p=2)
-    
-        This will return the indices of the closest points in `points_b` to each point in `points_a`.
-    """
-
-    # Convert tensors to numpy arrays
-    A_np = A.detach().numpy()
-    B_np = B.detach().numpy()
-    # Create Ball Tree and query with A
-    tree = BallTree(B_np, metric='minkowski', p=p)
-    _, ind = tree.query(A_np, k=1)
-    # Convert results back to tensor
-    return torch.tensor(ind.ravel())
-
-def find_longest_path(skeleton_pixels, initial_point):
-    r"""
-        Finds the longest path through a skeletonized representation of a binary image. This function constructs a directed graph from the 
-        skeleton pixels, with the skeleton treated as a graph where junctions and end points become nodes, and connections between them 
-        become directed edges. The function then calculates the longest path from a specified starting point to any node in the graph.
-    
-        The algorithm first identifies the closest skeleton pixel to an initial point and uses this as the starting node. It iteratively
-        builds the graph by traversing the skeleton, adding edges from each node to its connected neighbors, while avoiding cycles. Finally,
-        it utilizes the `dag_longest_path` method from `networkx` to determine the longest path in this directed acyclic graph (DAG).
-    
-        Arguments
-        ----------
-        skeleton_pixels : np.ndarray
-            A 2D array where each row corresponds to the coordinates of a skeleton pixel in the image.
-    
-        initial_point : np.ndarray
-            A 1D array representing the coordinates (x, y) of the initial point from which the nearest skeleton pixel is determined to start
-            the pathfinding process.
-    
-        Returns
-        -------
-        np.ndarray
-            An array of skeleton pixels representing the longest path found in the skeleton. Each row in the array is a pixel's coordinates
-            along this path.
-    
-        Example
-        -------
-        Given a skeleton represented by an array of pixels `skeleton` and an initial point `init_point`:
-            skeleton = np.array([[10, 10], [10, 11], [10, 12], [11, 12], [12, 12]])
-            init_point = np.array([10, 9])
-    
-        Finding the longest path:
-            longest_path = find_longest_path(skeleton, init_point)
-    
-        This would analyze the given skeleton structure, build the corresponding graph, and return the longest path starting from the
-        point in the skeleton closest to [10, 9].
-    """
-
-    # First build a directed graph of the skeleton
-    G = nx.DiGraph()
-    G.add_nodes_from(range(skeleton_pixels.shape[0]))
-    has_edge = np.zeros((skeleton_pixels.shape[0], ), dtype=bool)
-    
-    # Now add the edges starting from the skeleton pixel closest to initial_point
-    initial_index = np.argmin(np.linalg.norm(skeleton_pixels - initial_point, axis=1))
-    current_index = copy(initial_index)
-    has_edge[current_index] = True
-    bifurcation_points = [[current_index]]
-
-    # Now that the first path has been found iterate over the bifurcation points and add edges in the same way
-    for bifurcation in bifurcation_points:
-        current_index = int(bifurcation[0])
-        new_bifurcation_points = set_edges_branch(skeleton_pixels, current_index, has_edge, G, initial_index)
-        bifurcation_points.extend(new_bifurcation_points)
-    # Now that the graph is built, find the longest path
-    longest_path = nx.dag_longest_path(G)
-    return skeleton_pixels[longest_path, :]
-
-
-def set_edges_branch(skeleton_pixels: np.array, current_index: int, has_edge: np.array, G: nx.DiGraph, initial_index: int):
-    """
-        Checks one whole branch of the skeleton. By iteratively adding edges to the graph G by adding the next skeleton pixel to the graph. If there are multiple
-        skeleton pixels that are connected to the current skeleton pixel, the remaining ones are added to a list of bifurcation points that still need to be
-        checked. The algorithm returns a list of bifurcation points that still need to be checked.
-    """
-    bifurcation_points = []
-    while True:
-        # Find all the skeleton pixels that have an inf-norm distance to the current skeleton pixel of 1
-        current_pixel = skeleton_pixels[current_index, :]
-        next_pixels_bool = (np.linalg.norm(skeleton_pixels - current_pixel, axis=1, ord=np.inf) == 1) & (~has_edge)
-        next_pixels_idx = np.argwhere(next_pixels_bool)
-        if not all(next_pixels_idx.shape):
-            break
-        next_pixels = skeleton_pixels[next_pixels_idx, :]
-        # Now add edges to all the next pixels that have not been added yet
-        for i in range(next_pixels.shape[0]):
-            if current_index == initial_index:
-                # Ensure that the initial pixel is always contained in the path
-                G.add_edge(int(current_index), int(next_pixels_idx[i]), weight=1e8)
-                has_edge[next_pixels_idx[i]] = True
-            else:
-                G.add_edge(int(current_index), int(next_pixels_idx[i]))
-                has_edge[next_pixels_idx[i]] = True
-
-        # Check whether there are multiple skeleton pixels that are connected to the current skeleton pixel. If so, add them to the list of bifurcation points,
-        # excluding current_index.
-        if next_pixels_idx.shape[0] > 1:
-            # Set the current index to the index of the pixel from the next_pixels that follows the previous trend of the skeleton the best. This is done by
-            # computing the dot product of the vector from the current pixel to the next pixel with the vector from the previous 5 pixels to the current pixel.
-            # The pixel with the highest dot product is the one that follows the previous trend the best.
-            current_vectors = skeleton_pixels[current_index, :] - skeleton_pixels[current_index-5:current_index, :]
-            current_vector = np.mean(current_vectors / np.linalg.norm(current_vectors, axis=1)[:, None], axis=0)/np.linalg.norm(np.mean(current_vectors, axis=0))
-            next_vectors = skeleton_pixels[next_pixels_idx[:, 0], :] - skeleton_pixels[current_index, :]
-            next_vectors = next_vectors / np.linalg.norm(next_vectors, axis=1)[:, None]
-            current_index = int(next_pixels_idx[np.argmax(next_vectors @ current_vector.T), :])
-            bifurcation_points.append(next_pixels_idx[next_pixels_idx[:, 0] != current_index, :])
-        else:
-            current_index = int(next_pixels_idx[0])
-    return bifurcation_points
-
-
-def discretizeODE(odefun, method, dim, dt, s, x, dtype=casadi.MX):
-    r"""
-        Discretizes an ordinary differential equation (ODE) using a specified numerical integration method. This function is designed
-        to step through an ODE based on the initial conditions and parameters provided.
-    
-        This function primarily uses the Runge-Kutta method (or similar methods), parameterized by Butcher tableau coefficients to advance
-        the state of the system over a single time step. It computes the state of the system at the next time step by evaluating several
-        intermediate stages, each dependent on the results of the previous stages.
-    
-        .. note::
-            The function requires the Butcher tableau for the numerical method, which is an array detailing the coefficients used in the
-            numerical solution of ODEs. It supports any explicit Runge-Kutta method specified by its Butcher tableau.
-    
-        Arguments
-        ----------
-        odefun : callable
-            The function defining the ODE. It should take at least two arguments: time `s` and state `x`, and return the derivative of the state.
-    
-        method : str
-            The name of the integration method to use, which dictates the Butcher tableau. Integration method from the following list:
-    
-                - "rk1"/"euler"
-                - "rk2"/"midpoint"
-                - "heun"
-                - "rk3"/"simpson"
-                - "rk4"
-                - "3/8"
-                
-        dim : int
-            The dimension of the state vector `x`.
-    
-        dt : float
-            The time step to advance the solution.
-    
-        s : float
-            The current time.
-    
-        x : array_like
-            The current state vector of the system.
-    
-        dtype : data type, optional
-            The data type of the matrix that will hold the intermediate derivatives, by default `casadi.MX`, 
-            which is specific to CasADi's symbolic framework.
-    
-        Returns
-        -------
-        xplus : array_like
-            The state of the system at the next time step.
-    
-        Example
-        -------
-        Define an ODE function, such as a simple linear system:
-            def linear_system(t, x):
-                A = np.array([[0, 1], [-1, 0]])
-                return A @ x
-    
-        Using the RK4 method:
-            x_next = discretizeODE(linear_system, 'rk4', 2, 0.01, 1, 0, np.array([1, 0]))
-    
-        This would advance the system state from `np.array([1, 0])` at time `0` by `0.01` units using the RK4 integration method.
-    """
-
-    butcher = getMethod(method)
-    a = butcher[0:-1, 1:]
-    b = butcher[-1, 1:]
-    c = butcher[0:-1, 0]
-    
-    nStage = len(c)
-    k = dtype(dim, nStage)
-    
-    for iStage in range(nStage):
-        k[:, iStage] = odefun(s + dt*c[iStage], x + dt * k @ a[iStage,:].reshape(nStage, 1))
-        
-    xplus = x + dt * k @ b.reshape(nStage,1)
-    return xplus
-
-def getMethod(method):
-    r"""
-        Retrieves the Butcher tableau for a specified numerical integration method used in the solution of ordinary differential equations (ODEs).
-        The Butcher tableau is a matrix representation that includes all coefficients necessary for the Runge-Kutta methods or its variants.
-    
-        The function supports a variety of integration methods, each associated with specific coefficients that dictate the steps of the
-        integration process. These methods include simple Euler (first-order Runge-Kutta), Heun's method, Midpoint method (second-order Runge-Kutta),
-        classical fourth-order Runge-Kutta, and others like the three-eighths rule (another fourth-order method).
-    
-        .. note::
-            Each method is predefined with its respective coefficients arranged in a matrix format where the first row typically includes 
-            the time step coefficients (c), and the last row includes the weights for the final summation (b). Intermediate rows provide
-            the coefficients for the intermediate stages of the integration (a).
-    
-        Arguments
-        ----------
-        method : str
-            The name of the integration method. Integration method from the following list:
-    
-                - "rk1"/"euler"
-                - "rk2"/"midpoint"
-                - "heun"
-                - "rk3"/"simpson"
-                - "rk4"
-                - "3/8"
-    
-        Returns
-        -------
-        butcher : numpy.ndarray
-            The Butcher tableau as a NumPy array. This matrix contains all coefficients needed to implement the specified numerical integration method.
-    
-        Example
-        -------
-        Retrieve the Butcher tableau for the classical fourth-order Runge-Kutta method:
-            rk4_tableau = getMethod("rk4")
-    
-        This can be used to further implement the Runge-Kutta method for solving ODEs in a custom ODE solver.
-    """
-
-    if method == "rk1" or method == "euler":
-        butcher = np.diag([0,1])
-    
-    elif method == "rk2" or method == "midpoint":
-        butcher  = np.diag([0, 1/2, 1]) + np.diag([1/2, 0], -1)
-        
-    elif method == "heun":
-        butcher  = np.diag([0, 1, 1/2]) + np.diag([1, 1/2], -1)
-        
-    elif method == "rk3" or method == "simpson":
-        butcher = np.diag([0, 1/2, 2, 1/6]) + np.diag([1/2, -1, 2/3], -1) + np.diag([1, 1/6], -2)
-        
-    elif method == "rk4":
-        butcher = np.diag([0, 1/2, 1/2, 1, 1/6])
-        butcher[1:4, 0] = np.array([1, 1, 2])/2
-        butcher[-1, 1:4] = np.array([1, 2, 2])/6
-        
-    elif method == "3/8":
-        butcher = np.diag([0, 1/3, 1, 1, 1/8]) + np.diag([1/3, -1/3, -1, 3/8], -1) + \
-            np.diag([2/3, 1, 3/8], -2) + np.diag([1, 1/8], -3)
-        
-    return butcher
-
-
-def fromWorld2Img(pos, A, dist, P, R, T):
-    
-    r"""
-        Transforms 3D world coordinates into 2D pixel coordinates on an image plane using camera calibration parameters. This function
-        applies several transformations including a change from world coordinates to camera coordinates, normalization, and distortion
-        correction before finally using camera intrinsic parameters to map these points to pixel coordinates.
-    
-        The function ensures that all computations respect the data type required by PyTorch operations and handles both radial and
-        tangential distortions as part of the transformation process. The final output is the pixel coordinates that correspond to
-        the input 3D points as they would be captured by the camera.
-    
-        .. note::
-            This function is particularly useful in computer vision and robotics for tasks like object tracking, 3D reconstruction,
-            and augmented reality where accurate projection from 3D to 2D is crucial.
-    
-        Arguments
-        ----------
-        pos : torch.Tensor
-            A 3xN matrix of 3D world coordinates, where N is the number of points.
-    
-        A : torch.Tensor
-            The camera intrinsic matrix (3x3) including focal lengths and principal point.
-    
-        dist : tuple of floats
-            The distortion coefficients (k1, k2, p1, p2, k3) for radial and tangential distortion.
-    
-        P : torch.Tensor
-            The projection matrix (3x3) used to project 3D camera coordinates onto the image plane.
-    
-        R : torch.Tensor
-            The rotation matrix (3x3) describing the orientation of the camera in the world.
-    
-        T : torch.Tensor
-            The translation vector (3x1) describing the position of the camera in the world.
-    
-        Returns
-        -------
-        pixel : torch.Tensor
-            A 2xN matrix where each column represents the pixel coordinates of the corresponding 3D point in the image.
-    
-        Example
-        -------
-        Define world points, camera intrinsic matrix `A`, distortion coefficients, projection matrix `P`, rotation matrix `R`,
-        and translation vector `T`:
-            pos = torch.tensor([[1, 2, 3], [4, 5, 6], [7, 8, 9]], dtype=torch.float32)
-            A = torch.eye(3)
-            dist = (0.1, 0.01, 0.001, 0.001, 0.0001)
-            P = torch.eye(3)
-            R = torch.eye(3)
-            T = torch.tensor([0.1, 0.2, 0.3])
-    
-        Get pixel coordinates:
-            pixels = fromWorld2Img(pos, A, dist, P, R, T)
-    """
-
-    if pos.dtype != torch.float32:
-        pos = pos.float()
-   
-    R_t = torch.linalg.solve(A, P).float()
-    
-    # Convert from local coordinate system of the CR to the world coordinate system 
-    pos_camera = torch.linalg.solve(R, pos-T.reshape(3,1))
-
-    pos_camera_h = torch.concat((pos_camera, torch.ones((1, pos_camera.shape[1]))), 0)
-    
-    # Calculate normalized camera coordinates in Camera
-    camPoint = torch.matmul(R_t, pos_camera_h)
-    normCamPoint = camPoint[:2,:] / camPoint[2,:]
-
-    # Calculate Distortion
-    k1, k2, p1, p2, k3 = dist
-    r = normCamPoint[0,:]**2 + normCamPoint[1,:]**2 
-
-    radDist = 1.0 + k1*r + k2*r**2 + k3*r**3
-    tangDistX = 2*p1*normCamPoint[0,:]*normCamPoint[1] + p2*(r + 2*normCamPoint[0,:]**2)
-    tangDistY = p1*(r + 2*normCamPoint[1,:]**2) + 2*p2*normCamPoint[0,:]*normCamPoint[1,:]
-
-    # Add distortion
-    x = radDist*normCamPoint[0,:] + tangDistX
-    y = radDist*normCamPoint[1,:] + tangDistY
-
-    # Calculate pixel coordinates in Camera
-    pixel =  torch.matmul(A,torch.stack([x, y, torch.ones_like(x)],0))[:2]
-    
-    return pixel
-
-
-def fromWorld2ImgCasadi(pos, A, dist, P, R, T):
-    r"""
-        Transforms 3D world coordinates into 2D pixel coordinates using camera calibration parameters and the CasADi library for
-        numerical computations. This function is designed for applications in optimization and control where gradient computations are
-        necessary. It performs coordinate transformations, normalization, distortion correction, and final projection using camera
-        intrinsic parameters.
-    
-        This function leverages CasADi's symbolic capabilities to handle operations, making it suitable for scenarios where the
-        derivatives of the transformation process are needed for further optimizations.
-    
-        .. note::
-            The use of CasADi's `MX` data type and operations ensures that the function is compatible with CasADi's automatic differentiation,
-            which is crucial for gradient-based optimization tasks in computer vision and robotics.
-    
-        Arguments
-        ----------
-        pos : casadi.MX
-            A 3xN matrix of 3D world coordinates, where N is the number of points. Should be of type casadi.MX for compatibility.
-    
-        A : numpy.ndarray
-            The camera intrinsic matrix (3x3) including focal lengths and principal point. This is a static matrix.
-    
-        dist : tuple of floats
-            The distortion coefficients (k1, k2, p1, p2, k3) used to model radial and tangential distortions.
-    
-        P : numpy.ndarray
-            The projection matrix (3x3) used to project 3D camera coordinates onto the image plane. This is a static matrix.
-    
-        R : numpy.ndarray
-            The rotation matrix (3x3) describing the orientation of the camera in the world. This is a static matrix.
-    
-        T : numpy.ndarray
-            The translation vector (3x1) describing the position of the camera in the world. This is a static matrix.
-    
-        Returns
-        -------
-        pixel : casadi.MX
-            A 2xN matrix where each column represents the pixel coordinates of the corresponding 3D point in the image. The output is
-            of type casadi.MX to facilitate further symbolic operations if necessary.
-    
-        Example
-        -------
-        Define world points, camera intrinsic matrix `A`, distortion coefficients, projection matrix `P`, rotation matrix `R`,
-        and translation vector `T`:
-            pos = casadi.MX([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
-            A = np.eye(3)
-            dist = (0.1, 0.01, 0.001, 0.001, 0.0001)
-            P = np.eye(3)
-            R = np.eye(3)
-            T = np.array([0.1, 0.2, 0.3])
-    
-        Get pixel coordinates in a CasADi-compatible format:
-            pixels = fromWorld2ImgCasadi(pos, A, dist, P, R, T)
-    """
-
-    R_t = np.linalg.solve(A, P)
-    
-    # Convert from local coordinate system of the CR to the world coordinate system 
-    pos_camera = R.T@(pos-T.reshape(3,1)) # casadi.solve?
-
-    pos_camera_h = casadi.vertcat(pos_camera, casadi.MX.ones(1, pos_camera.shape[1]))
-    
-    # Calculate normalized camera coordinates in Camera
-    camPoint = R_t @ pos_camera_h
-    normCamPoint = camPoint[:2,:] / casadi.repmat(camPoint[2,:],2,1)
-
-    # Calculate Distortion
-    k1, k2, p1, p2, k3 = dist
-    r = normCamPoint[0,:]**2 + normCamPoint[1,:]**2 
-
-    radDist = 1.0 + k1*r + k2*r**2 + k3*r**3
-    tangDistX = 2*p1*normCamPoint[0,:]*normCamPoint[1,:] + p2*(r + 2*normCamPoint[0,:]**2)
-    tangDistY = p1*(r + 2*normCamPoint[1,:]**2) + 2*p2*normCamPoint[0,:]*normCamPoint[1,:]
-
-    # Add distortion
-    x = radDist*normCamPoint[0,:] + tangDistX
-    y = radDist*normCamPoint[1,:] + tangDistY
-
-    # Calculate pixel coordinates in Camera
-    pixel = (A @ casadi.vertcat(x, y, casadi.MX.ones(x.shape)))[:2,:]
-    
-    return pixel
-
-
-def spaceCarving(images, cam_params, x_bounds, y_bounds, z_bounds, resolution=0.001):
-    r"""
-        Performs space carving to reconstruct a 3D volume from multiple images based on visibility from different camera angles.
-        This method incrementally carves away the volume by projecting grid points into each image and checking if they are visible
-        in all images. Points that are visible in all images are retained, while others are discarded.
-    
-        The function uses a grid of points defined within specified bounds and checks these points against each provided image
-        using camera parameters to project 3D points into 2D image coordinates. Points that project outside the image bounds or
-        into areas that do not match the image data are considered occluded and are removed from consideration.
-    
-        Arguments
-        ----------
-        images : list of binary images
-            A list of images (2D arrays or tensors) from different views.
-    
-        cam_params : list of dicts
-            A list of dictionaries, where each dictionary contains the camera parameters needed by the `fromWorld2Img` function
-            to project 3D points onto each corresponding image. The dictionaries contain A, dist, p, R, and T.
-    
-        x_bounds : tuple of float
-            The lower and upper bounds in the x-axis within which the space carving is performed.
-    
-        y_bounds : tuple of float
-            The lower and upper bounds in the y-axis within which the space carving is performed.
-    
-        z_bounds : tuple of float
-            The lower and upper bounds in the z-axis within which the space carving is performed.
-    
-        resolution : float, optional
-            The resolution of the grid in all dimensions. Default is 0.001 units.
-    
-        Returns
-        -------
-        surviving_points : torch.Tensor
-            A tensor of 3D points that are visible in all images, representing the carved space.
-    
-        xgrid, ygrid, zgrid : torch.Tensor
-            The grid tensors in the x, y, and z dimensions respectively, which can be used for further analysis or visualization.
-    
-        Example
-        -------
-        Suppose you have multiple images and corresponding camera parameters:
-            images = [img1, img2, img3]  # list of PyTorch tensors
-            cam_params = [{'A': A1, 'dist': dist1, 'P': P1, 'R': R1, 'T': T1},
-                          {'A': A2, 'dist': dist2, 'P': P2, 'R': R2, 'T': T2},
-                          {'A': A3, 'dist': dist3, 'P': P3, 'R': R3, 'T': T3}]
-    
-        Define the bounds and resolution:
-            x_bounds = (-1, 1)
-            y_bounds = (-1, 1)
-            z_bounds = (-1, 1)
-            resolution = 0.01
-    
-        Perform space carving:
-            carved_points, xg, yg, zg = spaceCarving(images, cam_params, x_bounds, y_bounds, z_bounds, resolution)
-    """
-
-    xgrid, ygrid, zgrid = torch.meshgrid(torch.arange(x_bounds[0], x_bounds[1]+resolution, resolution), torch.arange(y_bounds[0], y_bounds[1]+resolution, resolution), torch.arange(z_bounds[0], z_bounds[1]+resolution, resolution), indexing='ij')
-    grid_points = torch.stack([xgrid.flatten(), ygrid.flatten(), zgrid.flatten()], 1)
-    voting = np.zeros((grid_points.shape[0], len(images)), bool)
-    for i in range(len(images)):
-        proj_pts = fromWorld2Img(grid_points.T, **cam_params[i]).round().T
-        filter_out = (proj_pts[:,0] < 0) | (proj_pts[:,1] < 0) | (proj_pts[:,0] >= images[i].shape[1]) | (proj_pts[:,1] >= images[i].shape[0])
-        grid_points = grid_points[~filter_out,:]
-        proj_pts = proj_pts[~filter_out,:]
-        voting = voting[~filter_out,:]
-        voting[:,i] = images[i][proj_pts[:,1].int(), proj_pts[:,0].int()]
-    return grid_points[voting.all(1),:], xgrid, ygrid, zgrid
-
-
-def spaceCarvingReconstruction(images, cam_params, p0=np.zeros((3,)), x_bounds=[-0.1, 0.1], y_bounds=[-0.1, 0.1], z_bounds=[0, 0.2], resolution=0.001):
-    r"""
-        Uses the spaceCarving method to generate a grid of 3D points potentially corresponding to the CR. The resulting grid is reduced to a skeleton that is
-        sorted using the find_longest_path method. Depending on the camera setup this is nevcessary to deal with ambiguous data, as it can happen with two images.
-    
-        Arguments
-        ----------
-        images : list of binary images
-            A list of 2D image tensors from different views, used to perform space carving.
-    
-        cam_params : list of dicts
-            A list of dictionaries where each dictionary contains camera parameters needed for projecting 3D points into the images.
-    
-        p0 : np.ndarray, optional
-            The origin point in 3D space from which to measure distances for pathfinding. Default is the zero vector (center of the bounds).
-    
-        x_bounds, y_bounds, z_bounds : list of float
-            The bounds in the x, y, and z dimensions respectively, defining the region within which the carving and reconstruction are performed.
-    
-        resolution : float, optional
-            The resolution of the grid in all dimensions, affecting the granularity of the carved space and the subsequent binary grid.
-            Default is 0.001 units.
-    
-        Returns
-        -------
-        tuple
-            Returns a tuple containing two elements:
-            path : torch.Tensor
-                A tensor containing the coordinates of the longest path found within the skeletonized grid. Useful for structural analysis.
-            pts_3d : torch.Tensor
-                The original point cloud derived from the space carving process before any skeletonization.
-    
-        Example
-        -------
-        Define a set of images and corresponding camera parameters:
-            images = [torch.rand(100, 100) for _ in range(5)]
-            cam_params = [{'A': torch.eye(3), 'dist': (0.1, 0.01, 0.001, 0.001, 0.0001), 'P': torch.eye(3), 'R': torch.eye(3), 'T': torch.tensor([0, 0, 0])} for _ in range(5)]
-    
-        Perform 3D reconstruction and analyze the structural properties:
-            path, pts_3d = spaceCarvingReconstruction(images, cam_params)
-    
-        This would compute the 3D structure, skeletonize it, and determine the longest path for analysis.
-    """
-
-    pts_3d, xgrid, ygrid, zgrid = spaceCarving(images, cam_params, x_bounds, y_bounds, z_bounds, resolution)
-
-    def get_binary_grid(pts_3d, x_bounds, y_bounds, z_bounds, resolution):
-        # Calculate grid size
-        grid_shape = (
-            int((x_bounds[1] - x_bounds[0]) / resolution) + 1,
-            int((y_bounds[1] - y_bounds[0]) / resolution) + 1,
-            int((z_bounds[1] - z_bounds[0]) / resolution) + 1
-        )
-        
-        # Initialize the binary grid
-        binary_3d_grid = torch.zeros(grid_shape, dtype=bool)
-        
-        # Convert pts_3d to grid indices
-        grid_indices = ((pts_3d - torch.tensor([x_bounds[0], y_bounds[0], z_bounds[0]])) / resolution).round().int()
-        
-        # Update the binary grid
-        for index in grid_indices:
-            binary_3d_grid[index[0], index[1], index[2]] = True
-        
-        return binary_3d_grid
-
-    binary_3d_grid = get_binary_grid(pts_3d, x_bounds, y_bounds, z_bounds, resolution)
-    skeletonized_grid = torch.from_numpy(skeletonize_3d(binary_3d_grid))
-
-    [xs, ys, zs] = torch.where(skeletonized_grid)
-    dist_grid = ((xgrid-p0[0])**2+(ygrid-p0[1])**2+(zgrid-p0[2])**2)
-    dist_min = torch.min(dist_grid)
-    initial_point_grid = torch.stack(torch.where(dist_grid == dist_min), 1)
-
-    path_grid = torch.from_numpy(find_longest_path(torch.stack((xs, ys, zs), 1).detach().numpy(), initial_point_grid.detach().numpy()))
-    path = torch.stack([xgrid[path_grid[:,0], path_grid[:,1], path_grid[:,2]], ygrid[path_grid[:,0], path_grid[:,1], path_grid[:,2]], zgrid[path_grid[:,0], path_grid[:,1], path_grid[:,2]]], 1)
-    path = torch.concatenate([torch.zeros((1,3)), path], 0)
-    
-    return path, pts_3d
-    
-"""
-    Alle Hilfsfunktionen
+import casadi
+import numpy as np
+import torch
+import networkx as nx
+from copy import copy
+from sklearn.neighbors import BallTree
+from torch.utils.data import Dataset
+from os.path import sep
+from skimage.morphology import skeletonize_3d
+
+def image_to_idx( img ):
+    """
+        Transform the binary image (img) to coordinates.
+    """
+    im_idc = np.where(img.T)
+    return np.stack(im_idc, 1)
+
+
+def camera_folder_to_params( camera_folder, cams, package="torch" ):
+    """
+        Read the parameters from a folder using predefined file names.
+
+        Arguments
+        ----------
+        camera_folder : str
+            Folder containing the parameter files.
+
+        cams : int or list
+            Either the number of cameras to be used or a list of camera indices.
+    """
+    i_cams = cams if type(cams) is list else list(range(cams))
+
+    param_list = []
+    path = camera_folder if camera_folder[-1] == sep else camera_folder + sep
+    load_and_tensor = {"torch":lambda x: torch.from_numpy(np.load(path + x)).float(), "casadi":lambda x: np.load(path + x)}[package]
+    for i in i_cams:
+        param_list.append({
+            "A": load_and_tensor(f"calib_A{i}.npy"),
+            "dist": load_and_tensor(f"calib_dist{i}.npy"),
+            "P": load_and_tensor(f"calib_P{i}_.npy"),
+            "R": load_and_tensor("cs_conversion_R.npy"),
+            "T": load_and_tensor("cs_conversion_T.npy")})
+    return param_list
+
+
+class PixelDataset(Dataset):
+    """
+        Dataset of all the pixel positions that correspond to the CR.
+
+        Arguments
+        ----------
+            p_list : list
+                List containing the pixel positions.
+
+        Returns
+        ----------
+            p : m-by-2 tensor
+                Tensor of pixel positions.
+
+            img_idx_data : m-by-1 tensor
+                Tensor containing the index of the corresponding camera.
+    """
+
+    def __init__( self, p_list ):
+        self.p = None
+        self.img_idx_data = None
+        for i in range(len(p_list)):
+            p = p_list[i]
+            self.p = p if self.p is None else np.concatenate((self.p, p), 0)
+            self.img_idx_data = i * np.ones((p.shape[0],), dtype=np.int8) if self.img_idx_data is None else np.concatenate(
+                (self.img_idx_data, i * np.ones((p.shape[0],), dtype=np.int8)), 0)
+
+    def __len__( self ):
+        return self.p.shape[0]
+
+    def __getitem__( self, idx ):
+        return (self.p[idx, :], self.img_idx_data[idx])
+
+def brute_force_distance_norm(A, B, p):
+    # Calculate distances using the p-norm
+    distances = torch.cdist(A, B, p=p)**p
+    # Find the index of the nearest point for each point in A
+    return distances, torch.argmin(distances, dim=1)
+
+def ball_tree_norm(A, B, p):
+    r"""
+        Efficiently finds the nearest neighbors from one set of points in A to another set in B using the Minkowski distance metric
+        parameterized by p. The function leverages a Ball Tree structure for fast nearest neighbor searches in high-dimensional spaces.
+    
+        The function converts PyTorch tensors to NumPy arrays, uses the BallTree implementation from sklearn for querying the nearest
+        neighbor, and finally converts the results back to a PyTorch tensor.
+    
+        Arguments
+        ----------
+        A : torch.Tensor
+            A tensor of points for which nearest neighbors in B need to be found. Each row corresponds to a different point.
+    
+        B : torch.Tensor
+            A tensor of points constituting the search space for nearest neighbors. Each row corresponds to a different point.
+    
+        p : int
+            The order of the Minkowski metric to be used for calculating distances. For example, p=2 corresponds to the Euclidean distance.
+    
+        Returns
+        -------
+        torch.Tensor
+            A tensor containing the indices of the nearest neighbors in B for each point in A. The indices are 1-dimensional (flattened).
+    
+        Example
+        -------
+        Suppose you have two sets of points, `points_a` and `points_b`, represented as PyTorch tensors:
+            points_a = torch.tensor([[1.0, 2.0], [2.0, 3.0]])
+            points_b = torch.tensor([[2.0, 1.0], [3.0, 2.0], [1.0, 2.0]])
+    
+        To find the nearest neighbor in `points_b` for each point in `points_a` using the Euclidean distance:
+            nearest_indices = ball_tree_norm(points_a, points_b, p=2)
+    
+        This will return the indices of the closest points in `points_b` to each point in `points_a`.
+    """
+
+    # Convert tensors to numpy arrays
+    A_np = A.detach().numpy()
+    B_np = B.detach().numpy()
+    # Create Ball Tree and query with A
+    tree = BallTree(B_np, metric='minkowski', p=p)
+    _, ind = tree.query(A_np, k=1)
+    # Convert results back to tensor
+    return torch.tensor(ind.ravel())
+
+def find_longest_path(skeleton_pixels, initial_point):
+    r"""
+        Finds the longest path through a skeletonized representation of a binary image. This function constructs a directed graph from the 
+        skeleton pixels, with the skeleton treated as a graph where junctions and end points become nodes, and connections between them 
+        become directed edges. The function then calculates the longest path from a specified starting point to any node in the graph.
+    
+        The algorithm first identifies the closest skeleton pixel to an initial point and uses this as the starting node. It iteratively
+        builds the graph by traversing the skeleton, adding edges from each node to its connected neighbors, while avoiding cycles. Finally,
+        it utilizes the `dag_longest_path` method from `networkx` to determine the longest path in this directed acyclic graph (DAG).
+    
+        Arguments
+        ----------
+        skeleton_pixels : np.ndarray
+            A 2D array where each row corresponds to the coordinates of a skeleton pixel in the image.
+    
+        initial_point : np.ndarray
+            A 1D array representing the coordinates (x, y) of the initial point from which the nearest skeleton pixel is determined to start
+            the pathfinding process.
+    
+        Returns
+        -------
+        np.ndarray
+            An array of skeleton pixels representing the longest path found in the skeleton. Each row in the array is a pixel's coordinates
+            along this path.
+    
+        Example
+        -------
+        Given a skeleton represented by an array of pixels `skeleton` and an initial point `init_point`:
+            skeleton = np.array([[10, 10], [10, 11], [10, 12], [11, 12], [12, 12]])
+            init_point = np.array([10, 9])
+    
+        Finding the longest path:
+            longest_path = find_longest_path(skeleton, init_point)
+    
+        This would analyze the given skeleton structure, build the corresponding graph, and return the longest path starting from the
+        point in the skeleton closest to [10, 9].
+    """
+
+    # First build a directed graph of the skeleton
+    G = nx.DiGraph()
+    G.add_nodes_from(range(skeleton_pixels.shape[0]))
+    has_edge = np.zeros((skeleton_pixels.shape[0], ), dtype=bool)
+    
+    # Now add the edges starting from the skeleton pixel closest to initial_point
+    initial_index = np.argmin(np.linalg.norm(skeleton_pixels - initial_point, axis=1))
+    current_index = copy(initial_index)
+    has_edge[current_index] = True
+    bifurcation_points = [[current_index]]
+
+    # Now that the first path has been found iterate over the bifurcation points and add edges in the same way
+    for bifurcation in bifurcation_points:
+        current_index = int(bifurcation[0])
+        new_bifurcation_points = set_edges_branch(skeleton_pixels, current_index, has_edge, G, initial_index)
+        bifurcation_points.extend(new_bifurcation_points)
+    # Now that the graph is built, find the longest path
+    longest_path = nx.dag_longest_path(G)
+    return skeleton_pixels[longest_path, :]
+
+
+def set_edges_branch(skeleton_pixels: np.array, current_index: int, has_edge: np.array, G: nx.DiGraph, initial_index: int):
+    """
+        Checks one whole branch of the skeleton. By iteratively adding edges to the graph G by adding the next skeleton pixel to the graph. If there are multiple
+        skeleton pixels that are connected to the current skeleton pixel, the remaining ones are added to a list of bifurcation points that still need to be
+        checked. The algorithm returns a list of bifurcation points that still need to be checked.
+    """
+    bifurcation_points = []
+    while True:
+        # Find all the skeleton pixels that have an inf-norm distance to the current skeleton pixel of 1
+        current_pixel = skeleton_pixels[current_index, :]
+        next_pixels_bool = (np.linalg.norm(skeleton_pixels - current_pixel, axis=1, ord=np.inf) == 1) & (~has_edge)
+        next_pixels_idx = np.argwhere(next_pixels_bool)
+        if not all(next_pixels_idx.shape):
+            break
+        next_pixels = skeleton_pixels[next_pixels_idx, :]
+        # Now add edges to all the next pixels that have not been added yet
+        for i in range(next_pixels.shape[0]):
+            if current_index == initial_index:
+                # Ensure that the initial pixel is always contained in the path
+                G.add_edge(int(current_index), int(next_pixels_idx[i]), weight=1e8)
+                has_edge[next_pixels_idx[i]] = True
+            else:
+                G.add_edge(int(current_index), int(next_pixels_idx[i]))
+                has_edge[next_pixels_idx[i]] = True
+
+        # Check whether there are multiple skeleton pixels that are connected to the current skeleton pixel. If so, add them to the list of bifurcation points,
+        # excluding current_index.
+        if next_pixels_idx.shape[0] > 1:
+            # Set the current index to the index of the pixel from the next_pixels that follows the previous trend of the skeleton the best. This is done by
+            # computing the dot product of the vector from the current pixel to the next pixel with the vector from the previous 5 pixels to the current pixel.
+            # The pixel with the highest dot product is the one that follows the previous trend the best.
+            current_vectors = skeleton_pixels[current_index, :] - skeleton_pixels[current_index-5:current_index, :]
+            current_vector = np.mean(current_vectors / np.linalg.norm(current_vectors, axis=1)[:, None], axis=0)/np.linalg.norm(np.mean(current_vectors, axis=0))
+            next_vectors = skeleton_pixels[next_pixels_idx[:, 0], :] - skeleton_pixels[current_index, :]
+            next_vectors = next_vectors / np.linalg.norm(next_vectors, axis=1)[:, None]
+            current_index = int(next_pixels_idx[np.argmax(next_vectors @ current_vector.T), :])
+            bifurcation_points.append(next_pixels_idx[next_pixels_idx[:, 0] != current_index, :])
+        else:
+            current_index = int(next_pixels_idx[0])
+    return bifurcation_points
+
+
+def discretizeODE(odefun, method, dim, dt, s, x, dtype=casadi.MX):
+    r"""
+        Discretizes an ordinary differential equation (ODE) using a specified numerical integration method. This function is designed
+        to step through an ODE based on the initial conditions and parameters provided.
+    
+        This function primarily uses the Runge-Kutta method (or similar methods), parameterized by Butcher tableau coefficients to advance
+        the state of the system over a single time step. It computes the state of the system at the next time step by evaluating several
+        intermediate stages, each dependent on the results of the previous stages.
+    
+        .. note::
+            The function requires the Butcher tableau for the numerical method, which is an array detailing the coefficients used in the
+            numerical solution of ODEs. It supports any explicit Runge-Kutta method specified by its Butcher tableau.
+    
+        Arguments
+        ----------
+        odefun : callable
+            The function defining the ODE. It should take at least two arguments: time `s` and state `x`, and return the derivative of the state.
+    
+        method : str
+            The name of the integration method to use, which dictates the Butcher tableau. Integration method from the following list:
+    
+                - "rk1"/"euler"
+                - "rk2"/"midpoint"
+                - "heun"
+                - "rk3"/"simpson"
+                - "rk4"
+                - "3/8"
+                
+        dim : int
+            The dimension of the state vector `x`.
+    
+        dt : float
+            The time step to advance the solution.
+    
+        s : float
+            The current time.
+    
+        x : array_like
+            The current state vector of the system.
+    
+        dtype : data type, optional
+            The data type of the matrix that will hold the intermediate derivatives, by default `casadi.MX`, 
+            which is specific to CasADi's symbolic framework.
+    
+        Returns
+        -------
+        xplus : array_like
+            The state of the system at the next time step.
+    
+        Example
+        -------
+        Define an ODE function, such as a simple linear system:
+            def linear_system(t, x):
+                A = np.array([[0, 1], [-1, 0]])
+                return A @ x
+    
+        Using the RK4 method:
+            x_next = discretizeODE(linear_system, 'rk4', 2, 0.01, 1, 0, np.array([1, 0]))
+    
+        This would advance the system state from `np.array([1, 0])` at time `0` by `0.01` units using the RK4 integration method.
+    """
+
+    butcher = getMethod(method)
+    a = butcher[0:-1, 1:]
+    b = butcher[-1, 1:]
+    c = butcher[0:-1, 0]
+    
+    nStage = len(c)
+    k = dtype(dim, nStage)
+    
+    for iStage in range(nStage):
+        k[:, iStage] = odefun(s + dt*c[iStage], x + dt * k @ a[iStage,:].reshape(nStage, 1))
+        
+    xplus = x + dt * k @ b.reshape(nStage,1)
+    return xplus
+
+def getMethod(method):
+    r"""
+        Retrieves the Butcher tableau for a specified numerical integration method used in the solution of ordinary differential equations (ODEs).
+        The Butcher tableau is a matrix representation that includes all coefficients necessary for the Runge-Kutta methods or its variants.
+    
+        The function supports a variety of integration methods, each associated with specific coefficients that dictate the steps of the
+        integration process. These methods include simple Euler (first-order Runge-Kutta), Heun's method, Midpoint method (second-order Runge-Kutta),
+        classical fourth-order Runge-Kutta, and others like the three-eighths rule (another fourth-order method).
+    
+        .. note::
+            Each method is predefined with its respective coefficients arranged in a matrix format where the first row typically includes 
+            the time step coefficients (c), and the last row includes the weights for the final summation (b). Intermediate rows provide
+            the coefficients for the intermediate stages of the integration (a).
+    
+        Arguments
+        ----------
+        method : str
+            The name of the integration method. Integration method from the following list:
+    
+                - "rk1"/"euler"
+                - "rk2"/"midpoint"
+                - "heun"
+                - "rk3"/"simpson"
+                - "rk4"
+                - "3/8"
+    
+        Returns
+        -------
+        butcher : numpy.ndarray
+            The Butcher tableau as a NumPy array. This matrix contains all coefficients needed to implement the specified numerical integration method.
+    
+        Example
+        -------
+        Retrieve the Butcher tableau for the classical fourth-order Runge-Kutta method:
+            rk4_tableau = getMethod("rk4")
+    
+        This can be used to further implement the Runge-Kutta method for solving ODEs in a custom ODE solver.
+    """
+
+    if method == "rk1" or method == "euler":
+        butcher = np.diag([0,1])
+    
+    elif method == "rk2" or method == "midpoint":
+        butcher  = np.diag([0, 1/2, 1]) + np.diag([1/2, 0], -1)
+        
+    elif method == "heun":
+        butcher  = np.diag([0, 1, 1/2]) + np.diag([1, 1/2], -1)
+        
+    elif method == "rk3" or method == "simpson":
+        butcher = np.diag([0, 1/2, 2, 1/6]) + np.diag([1/2, -1, 2/3], -1) + np.diag([1, 1/6], -2)
+        
+    elif method == "rk4":
+        butcher = np.diag([0, 1/2, 1/2, 1, 1/6])
+        butcher[1:4, 0] = np.array([1, 1, 2])/2
+        butcher[-1, 1:4] = np.array([1, 2, 2])/6
+        
+    elif method == "3/8":
+        butcher = np.diag([0, 1/3, 1, 1, 1/8]) + np.diag([1/3, -1/3, -1, 3/8], -1) + \
+            np.diag([2/3, 1, 3/8], -2) + np.diag([1, 1/8], -3)
+        
+    return butcher
+
+
+def fromWorld2Img(pos, A, dist, P, R, T):
+    
+    r"""
+        Transforms 3D world coordinates into 2D pixel coordinates on an image plane using camera calibration parameters. This function
+        applies several transformations including a change from world coordinates to camera coordinates, normalization, and distortion
+        correction before finally using camera intrinsic parameters to map these points to pixel coordinates.
+    
+        The function ensures that all computations respect the data type required by PyTorch operations and handles both radial and
+        tangential distortions as part of the transformation process. The final output is the pixel coordinates that correspond to
+        the input 3D points as they would be captured by the camera.
+    
+        .. note::
+            This function is particularly useful in computer vision and robotics for tasks like object tracking, 3D reconstruction,
+            and augmented reality where accurate projection from 3D to 2D is crucial.
+    
+        Arguments
+        ----------
+        pos : torch.Tensor
+            A 3xN matrix of 3D world coordinates, where N is the number of points.
+    
+        A : torch.Tensor
+            The camera intrinsic matrix (3x3) including focal lengths and principal point.
+    
+        dist : tuple of floats
+            The distortion coefficients (k1, k2, p1, p2, k3) for radial and tangential distortion.
+    
+        P : torch.Tensor
+            The projection matrix (3x4) used to project 3D camera coordinates onto the image plane.
+    
+        R : torch.Tensor
+            The rotation matrix (3x3) describing the orientation of the first camera in world coordinates.
+    
+        T : torch.Tensor
+            The translation vector (3x1) describing the position of the first camera in world coordinates.
+    
+        Returns
+        -------
+        pixel : torch.Tensor
+            A 2xN matrix where each column represents the pixel coordinates of the corresponding 3D point in the image.
+    
+        Example
+        -------
+        Define world points, camera intrinsic matrix `A`, distortion coefficients, projection matrix `P`, rotation matrix `R`,
+        and translation vector `T`:
+            pos = torch.tensor([[1, 2, 3], [4, 5, 6], [7, 8, 9]], dtype=torch.float32)
+            A = torch.eye(3)
+            dist = (0.1, 0.01, 0.001, 0.001, 0.0001)
+            P = torch.eye(3)
+            R = torch.eye(3)
+            T = torch.tensor([0.1, 0.2, 0.3])
+    
+        Get pixel coordinates:
+            pixels = fromWorld2Img(pos, A, dist, P, R, T)
+    """
+
+    if pos.dtype != torch.float32:
+        pos = pos.float()
+   
+    R_t = torch.linalg.solve(A, P).float()
+    
+    # Convert from local coordinate system of the CR to the world coordinate system 
+    pos_camera = R.T@(pos-T.reshape(3,1))
+    pos_camera_h = torch.concat((pos_camera, torch.ones((1, pos_camera.shape[1]))), 0)
+    
+    # Calculate normalized camera coordinates in Camera
+    camPoint = torch.matmul(R_t, pos_camera_h)
+    normCamPoint = camPoint[:2,:] / camPoint[2,:]
+
+    # Distort image
+    k1, k2, p1, p2, k3 = dist
+    r_sq = normCamPoint[0,:]**2 + normCamPoint[1,:]**2 
+
+    radDist = 1.0 + k1*r_sq + k2*r_sq**2 + k3*r_sq**3
+    tangDistX = 2*p1*normCamPoint[0,:]*normCamPoint[1] + p2*(r_sq + 2*normCamPoint[0,:]**2)
+    tangDistY = p1*(r_sq + 2*normCamPoint[1,:]**2) + 2*p2*normCamPoint[0,:]*normCamPoint[1,:]
+
+    # Add distortion
+    x = radDist*normCamPoint[0,:] + tangDistX
+    y = radDist*normCamPoint[1,:] + tangDistY
+
+    # Calculate pixel coordinates in Camera
+    pixel = torch.matmul(A, torch.stack([x, y, torch.ones_like(x)],0))[:2]
+    
+    return pixel
+
+
+def fromWorld2ImgCasadi(pos, A, dist, P, R, T):
+    r"""
+        Transforms 3D world coordinates into 2D pixel coordinates using camera calibration parameters and the CasADi library for
+        numerical computations. This function is designed for applications in optimization and control where gradient computations are
+        necessary. It performs coordinate transformations, normalization, distortion correction, and final projection using camera
+        intrinsic parameters.
+    
+        This function leverages CasADi's symbolic capabilities to handle operations, making it suitable for scenarios where the
+        derivatives of the transformation process are needed for further optimizations.
+    
+        .. note::
+            The use of CasADi's `MX` data type and operations ensures that the function is compatible with CasADi's automatic differentiation,
+            which is crucial for gradient-based optimization tasks in computer vision and robotics.
+    
+        Arguments
+        ----------
+        pos : casadi.MX
+            A 3xN matrix of 3D world coordinates, where N is the number of points. Should be of type casadi.MX for compatibility.
+    
+        A : numpy.ndarray
+            The camera intrinsic matrix (3x3) including focal lengths and principal point. This is a static matrix.
+    
+        dist : tuple of floats
+            The distortion coefficients (k1, k2, p1, p2, k3) used to model radial and tangential distortions.
+    
+        P : numpy.ndarray
+            The projection matrix (3x3) used to project 3D camera coordinates onto the image plane. This is a static matrix.
+    
+        R : numpy.ndarray
+            The rotation matrix (3x3) describing the orientation of the first camera in world coordinates.
+    
+        T : numpy.ndarray
+            The translation vector (3x1) describing the position of the first camera in world coordinates.
+    
+        Returns
+        -------
+        pixel : casadi.MX
+            A 2xN matrix where each column represents the pixel coordinates of the corresponding 3D point in the image. The output is
+            of type casadi.MX to facilitate further symbolic operations if necessary.
+    
+        Example
+        -------
+        Define world points, camera intrinsic matrix `A`, distortion coefficients, projection matrix `P`, rotation matrix `R`,
+        and translation vector `T`:
+            pos = casadi.MX([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
+            A = np.eye(3)
+            dist = (0.1, 0.01, 0.001, 0.001, 0.0001)
+            P = np.eye(3)
+            R = np.eye(3)
+            T = np.array([0.1, 0.2, 0.3])
+    
+        Get pixel coordinates in a CasADi-compatible format:
+            pixels = fromWorld2ImgCasadi(pos, A, dist, P, R, T)
+    """
+
+    R_t = np.linalg.solve(A, P)
+    
+    # Convert from local coordinate system of the CR to the world coordinate system 
+    pos_camera = R.T@(pos-T.reshape(3,1))
+
+    pos_camera_h = casadi.vertcat(pos_camera, casadi.MX.ones(1, pos_camera.shape[1]))
+    
+    # Calculate normalized camera coordinates in Camera
+    camPoint = R_t @ pos_camera_h
+    normCamPoint = camPoint[:2,:] / casadi.repmat(camPoint[2,:],2,1)
+
+    # Calculate Distortion
+    k1, k2, p1, p2, k3 = dist
+    r = normCamPoint[0,:]**2 + normCamPoint[1,:]**2 
+
+    radDist = 1.0 + k1*r + k2*r**2 + k3*r**3
+    tangDistX = 2*p1*normCamPoint[0,:]*normCamPoint[1,:] + p2*(r + 2*normCamPoint[0,:]**2)
+    tangDistY = p1*(r + 2*normCamPoint[1,:]**2) + 2*p2*normCamPoint[0,:]*normCamPoint[1,:]
+
+    # Add distortion
+    x = radDist*normCamPoint[0,:] + tangDistX
+    y = radDist*normCamPoint[1,:] + tangDistY
+
+    # Calculate pixel coordinates in Camera
+    pixel = (A @ casadi.vertcat(x, y, casadi.MX.ones(x.shape)))[:2,:]
+    
+    return pixel
+
+
+def spaceCarving(images, cam_params, x_bounds, y_bounds, z_bounds, resolution=0.001):
+    r"""
+        Performs space carving to reconstruct a 3D volume from multiple images based on visibility from different camera angles.
+        This method incrementally carves away the volume by projecting grid points into each image and checking if they are visible
+        in all images. Points that are visible in all images are retained, while others are discarded.
+    
+        The function uses a grid of points defined within specified bounds and checks these points against each provided image
+        using camera parameters to project 3D points into 2D image coordinates. Points that project outside the image bounds or
+        into areas that do not match the image data are considered occluded and are removed from consideration.
+    
+        Arguments
+        ----------
+        images : list of binary images
+            A list of images (2D arrays or tensors) from different views.
+    
+        cam_params : list of dicts
+            A list of dictionaries, where each dictionary contains the camera parameters needed by the `fromWorld2Img` function
+            to project 3D points onto each corresponding image. The dictionaries contain A, dist, p, R, and T.
+    
+        x_bounds : tuple of float
+            The lower and upper bounds in the x-axis within which the space carving is performed.
+    
+        y_bounds : tuple of float
+            The lower and upper bounds in the y-axis within which the space carving is performed.
+    
+        z_bounds : tuple of float
+            The lower and upper bounds in the z-axis within which the space carving is performed.
+    
+        resolution : float, optional
+            The resolution of the grid in all dimensions. Default is 0.001 units.
+    
+        Returns
+        -------
+        surviving_points : torch.Tensor
+            A tensor of 3D points that are visible in all images, representing the carved space.
+    
+        xgrid, ygrid, zgrid : torch.Tensor
+            The grid tensors in the x, y, and z dimensions respectively, which can be used for further analysis or visualization.
+    
+        Example
+        -------
+        Suppose you have multiple images and corresponding camera parameters:
+            images = [img1, img2, img3]  # list of PyTorch tensors
+            cam_params = [{'A': A1, 'dist': dist1, 'P': P1, 'R': R1, 'T': T1},
+                          {'A': A2, 'dist': dist2, 'P': P2, 'R': R2, 'T': T2},
+                          {'A': A3, 'dist': dist3, 'P': P3, 'R': R3, 'T': T3}]
+    
+        Define the bounds and resolution:
+            x_bounds = (-1, 1)
+            y_bounds = (-1, 1)
+            z_bounds = (-1, 1)
+            resolution = 0.01
+    
+        Perform space carving:
+            carved_points, xg, yg, zg = spaceCarving(images, cam_params, x_bounds, y_bounds, z_bounds, resolution)
+    """
+
+    xgrid, ygrid, zgrid = torch.meshgrid(torch.arange(x_bounds[0], x_bounds[1]+resolution, resolution), torch.arange(y_bounds[0], y_bounds[1]+resolution, resolution), torch.arange(z_bounds[0], z_bounds[1]+resolution, resolution), indexing='ij')
+    grid_points = torch.stack([xgrid.flatten(), ygrid.flatten(), zgrid.flatten()], 1)
+    voting = np.zeros((grid_points.shape[0], len(images)), bool)
+    for i in range(len(images)):
+        proj_pts = fromWorld2Img(grid_points.T, **cam_params[i]).round().T
+        filter_out = (proj_pts[:,0] < 0) | (proj_pts[:,1] < 0) | (proj_pts[:,0] >= images[i].shape[1]) | (proj_pts[:,1] >= images[i].shape[0])
+        grid_points = grid_points[~filter_out,:]
+        proj_pts = proj_pts[~filter_out,:]
+        voting = voting[~filter_out,:]
+        voting[:,i] = images[i][proj_pts[:,1].int(), proj_pts[:,0].int()]
+    return grid_points[voting.all(1),:], xgrid, ygrid, zgrid
+
+
+def spaceCarvingReconstruction(images, cam_params, p0=np.zeros((3,)), x_bounds=[-0.1, 0.1], y_bounds=[-0.1, 0.1], z_bounds=[0, 0.2], resolution=0.001):
+    r"""
+        Uses the spaceCarving method to generate a grid of 3D points potentially corresponding to the CR. The resulting grid is reduced to a skeleton that is
+        sorted using the find_longest_path method. Depending on the camera setup this is nevcessary to deal with ambiguous data, as it can happen with two images.
+    
+        Arguments
+        ----------
+        images : list of binary images
+            A list of 2D image tensors from different views, used to perform space carving.
+    
+        cam_params : list of dicts
+            A list of dictionaries where each dictionary contains camera parameters needed for projecting 3D points into the images.
+    
+        p0 : np.ndarray, optional
+            The origin point in 3D space from which to measure distances for pathfinding. Default is the zero vector (center of the bounds).
+    
+        x_bounds, y_bounds, z_bounds : list of float
+            The bounds in the x, y, and z dimensions respectively, defining the region within which the carving and reconstruction are performed.
+    
+        resolution : float, optional
+            The resolution of the grid in all dimensions, affecting the granularity of the carved space and the subsequent binary grid.
+            Default is 0.001 units.
+    
+        Returns
+        -------
+        tuple
+            Returns a tuple containing two elements:
+            path : torch.Tensor
+                A tensor containing the coordinates of the longest path found within the skeletonized grid. Useful for structural analysis.
+            pts_3d : torch.Tensor
+                The original point cloud derived from the space carving process before any skeletonization.
+    
+        Example
+        -------
+        Define a set of images and corresponding camera parameters:
+            images = [torch.rand(100, 100) for _ in range(5)]
+            cam_params = [{'A': torch.eye(3), 'dist': (0.1, 0.01, 0.001, 0.001, 0.0001), 'P': torch.eye(3), 'R': torch.eye(3), 'T': torch.tensor([0, 0, 0])} for _ in range(5)]
+    
+        Perform 3D reconstruction and analyze the structural properties:
+            path, pts_3d = spaceCarvingReconstruction(images, cam_params)
+    
+        This would compute the 3D structure, skeletonize it, and determine the longest path for analysis.
+    """
+
+    pts_3d, xgrid, ygrid, zgrid = spaceCarving(images, cam_params, x_bounds, y_bounds, z_bounds, resolution)
+
+    def get_binary_grid(pts_3d, x_bounds, y_bounds, z_bounds, resolution):
+        # Calculate grid size
+        grid_shape = (
+            int((x_bounds[1] - x_bounds[0]) / resolution) + 1,
+            int((y_bounds[1] - y_bounds[0]) / resolution) + 1,
+            int((z_bounds[1] - z_bounds[0]) / resolution) + 1
+        )
+        
+        # Initialize the binary grid
+        binary_3d_grid = torch.zeros(grid_shape, dtype=bool)
+        
+        # Convert pts_3d to grid indices
+        grid_indices = ((pts_3d - torch.tensor([x_bounds[0], y_bounds[0], z_bounds[0]])) / resolution).round().int()
+        
+        # Update the binary grid
+        for index in grid_indices:
+            binary_3d_grid[index[0], index[1], index[2]] = True
+        
+        return binary_3d_grid
+
+    binary_3d_grid = get_binary_grid(pts_3d, x_bounds, y_bounds, z_bounds, resolution)
+    skeletonized_grid = torch.from_numpy(skeletonize_3d(binary_3d_grid))
+
+    [xs, ys, zs] = torch.where(skeletonized_grid)
+    dist_grid = ((xgrid-p0[0])**2+(ygrid-p0[1])**2+(zgrid-p0[2])**2)
+    dist_min = torch.min(dist_grid)
+    initial_point_grid = torch.stack(torch.where(dist_grid == dist_min), 1)
+
+    path_grid = torch.from_numpy(find_longest_path(torch.stack((xs, ys, zs), 1).detach().numpy(), initial_point_grid.detach().numpy()))
+    path = torch.stack([xgrid[path_grid[:,0], path_grid[:,1], path_grid[:,2]], ygrid[path_grid[:,0], path_grid[:,1], path_grid[:,2]], zgrid[path_grid[:,0], path_grid[:,1], path_grid[:,2]]], 1)
+    path = torch.concatenate([torch.zeros((1,3)), path], 0)
+    
+    return path, pts_3d
+    
+"""
+    Alle Hilfsfunktionen
 """
```

