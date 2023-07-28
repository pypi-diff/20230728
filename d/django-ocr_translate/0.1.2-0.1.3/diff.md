# Comparing `tmp/django_ocr_translate-0.1.2.tar.gz` & `tmp/django_ocr_translate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ocr_translate-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_ocr_translate-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_ocr_translate-0.1.2.tar` & `django_ocr_translate-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,30 @@
--rw-r--r--   0        0        0    35148 2023-07-17 13:36:44.599288 django_ocr_translate-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0    11251 2023-07-18 15:09:28.584490 django_ocr_translate-0.1.2/README.md
--rw-r--r--   0        0        0     5129 2023-07-18 08:48:23.009143 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/__init__.py
--rw-r--r--   0        0        0     5488 2023-07-18 14:51:14.397771 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/base.py
--rw-r--r--   0        0        0     5846 2023-07-18 08:49:34.424167 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/box.py
--rw-r--r--   0        0        0     1937 2023-07-18 08:49:42.812053 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/lang.py
--rw-r--r--   0        0        0    31397 2023-07-17 08:16:48.861211 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/languages.json
--rw-r--r--   0        0        0     3470 2023-07-14 08:55:42.668357 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/models.json
--rw-r--r--   0        0        0     5936 2023-07-18 08:49:48.831971 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/ocr.py
--rw-r--r--   0        0        0     4484 2023-07-18 08:55:01.567722 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/tesseract.py
--rw-r--r--   0        0        0     7310 2023-07-18 08:49:59.215829 django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/tsl.py
--rw-r--r--   0        0        0     1535 2023-07-18 08:47:45.673654 django_ocr_translate-0.1.2/ocr_translate/__init__.py
--rw-r--r--   0        0        0     2110 2023-07-18 08:47:49.617600 django_ocr_translate-0.1.2/ocr_translate/admin.py
--rw-r--r--   0        0        0     1664 2023-07-18 08:47:53.393548 django_ocr_translate-0.1.2/ocr_translate/apps.py
--rw-r--r--   0        0        0    10798 2023-07-18 08:47:57.465492 django_ocr_translate-0.1.2/ocr_translate/messaging.py
--rw-r--r--   0        0        0     7367 2023-07-17 14:12:36.986612 django_ocr_translate-0.1.2/ocr_translate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-03 09:20:12.029899 django_ocr_translate-0.1.2/ocr_translate/migrations/__init__.py
--rw-r--r--   0        0        0     6297 2023-07-18 08:48:01.365439 django_ocr_translate-0.1.2/ocr_translate/models.py
--rw-r--r--   0        0        0     2239 2023-07-18 08:48:04.989389 django_ocr_translate-0.1.2/ocr_translate/queues.py
--rw-r--r--   0        0        0       60 2023-07-03 09:20:12.029899 django_ocr_translate-0.1.2/ocr_translate/tests.py
--rw-r--r--   0        0        0     1861 2023-07-18 11:20:28.894175 django_ocr_translate-0.1.2/ocr_translate/urls.py
--rw-r--r--   0        0        0    10806 2023-07-18 11:43:32.656054 django_ocr_translate-0.1.2/ocr_translate/views.py
--rw-r--r--   0        0        0     2177 2023-07-18 08:20:10.547589 django_ocr_translate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       72 2023-07-11 14:09:27.469500 django_ocr_translate-0.1.2/requirements-torch-cpu.txt
--rw-r--r--   0        0        0       32 2023-07-17 15:34:29.789228 django_ocr_translate-0.1.2/requirements-torch-cuda.txt
--rw-r--r--   0        0        0      284 2023-07-17 16:39:05.386922 django_ocr_translate-0.1.2/requirements.txt
--rw-r--r--   0        0        0    12798 1970-01-01 00:00:00.000000 django_ocr_translate-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1152 2023-07-27 00:26:54.434847 django_ocr_translate-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    35821 2023-07-17 20:52:55.210676 django_ocr_translate-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0    12769 2023-07-27 21:45:27.432567 django_ocr_translate-0.1.3/README.md
+-rw-r--r--   0        0        0      761 2023-07-27 21:10:13.816065 django_ocr_translate-0.1.3/build.sh
+-rw-r--r--   0        0        0     1593 2023-07-27 21:30:15.182242 django_ocr_translate-0.1.3/ocr_translate/__init__.py
+-rw-r--r--   0        0        0     2354 2023-07-27 00:26:54.442034 django_ocr_translate-0.1.3/ocr_translate/admin.py
+-rw-r--r--   0        0        0     1779 2023-07-27 00:26:54.443334 django_ocr_translate-0.1.3/ocr_translate/apps.py
+-rw-r--r--   0        0        0    15700 2023-07-27 17:52:11.399422 django_ocr_translate-0.1.3/ocr_translate/messaging.py
+-rw-r--r--   0        0        0     7500 2023-07-17 20:52:55.232594 django_ocr_translate-0.1.3/ocr_translate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-17 20:52:55.234224 django_ocr_translate-0.1.3/ocr_translate/migrations/__init__.py
+-rw-r--r--   0        0        0     6533 2023-07-27 00:26:54.445903 django_ocr_translate-0.1.3/ocr_translate/models.py
+-rw-r--r--   0        0        0     2017 2023-07-27 17:52:11.403664 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/__init__.py
+-rw-r--r--   0        0        0     8816 2023-07-27 17:52:11.406532 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/box.py
+-rw-r--r--   0        0        0     4424 2023-07-27 00:26:54.450181 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/full.py
+-rw-r--r--   0        0        0     3918 2023-07-27 17:52:11.410024 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/huggingface.py
+-rw-r--r--   0        0        0     5068 2023-07-27 17:52:11.410530 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/initializers.py
+-rw-r--r--   0        0        0     2111 2023-07-27 00:26:54.451236 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/lang.py
+-rw-r--r--   0        0        0    32920 2023-07-27 00:26:54.452276 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/languages.json
+-rw-r--r--   0        0        0     3528 2023-07-27 00:26:54.452676 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/models.json
+-rw-r--r--   0        0        0     8183 2023-07-27 17:52:11.414152 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/ocr.py
+-rw-r--r--   0        0        0     5361 2023-07-27 17:52:11.414152 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/tesseract.py
+-rw-r--r--   0        0        0    10549 2023-07-27 17:52:11.427554 django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/tsl.py
+-rw-r--r--   0        0        0     2331 2023-07-27 00:26:54.455809 django_ocr_translate-0.1.3/ocr_translate/queues.py
+-rw-r--r--   0        0        0     2048 2023-07-27 00:26:54.458525 django_ocr_translate-0.1.3/ocr_translate/urls.py
+-rw-r--r--   0        0        0    12645 2023-07-27 00:26:54.459099 django_ocr_translate-0.1.3/ocr_translate/views.py
+-rw-r--r--   0        0        0     2950 2023-07-28 01:13:53.148150 django_ocr_translate-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-07-27 00:26:54.461174 django_ocr_translate-0.1.3/requirements-torch-cpu.txt
+-rw-r--r--   0        0        0       76 2023-07-27 21:10:13.818678 django_ocr_translate-0.1.3/requirements-torch-cuda.txt
+-rw-r--r--   0        0        0      301 2023-07-27 00:26:54.463254 django_ocr_translate-0.1.3/requirements.txt
+-rw-r--r--   0        0        0    14672 1970-01-01 00:00:00.000000 django_ocr_translate-0.1.3/PKG-INFO
```

### Comparing `django_ocr_translate-0.1.2/LICENSE.txt` & `django_ocr_translate-0.1.3/LICENSE.txt`

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
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `django_ocr_translate-0.1.2/README.md` & `django_ocr_translate-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,177 +1,195 @@
-# OCR_translate
-
-This is a Django app for creating back-end server aimed at performing OCR and translation of images received via a POST request.
-
-The OCR and translation is performed using freely available machine learning models and packages (see below for what is currently implemented).
-
-The server is designed to be used together with [this browser extension](https://github.com/Crivella/ocr_extension), acting as a front-end providing the images and controlling the model languages and models being used.
-
-## Installation
-
-It is strongly suggested to install this project using a [virtual environment](https://docs.python.org/3/library/venv.html).
-
-### From Github
-
-- Clone or download the repository
-  - `git clone https://github.com/Crivella/ocr_translate.git`
-- Install the project dependencies (choose the appropriate files depending if you wanna run on GPU or CPU only):
-  - `pip install -r requirements-torch-[cpu/cuda].txt`
-  - `pip install -r requirements.txt`
-
-### From Docker
-Plan to add a CPU and a CUDA specific image to DockerHUB.
-For now you can create the image yourself by:
-
-- Create a .pip-cache-cpu directory inside your project.
-- Optional: re-install the project dependencies pointing this as the cache folder for pip (will make the build process much faster, by reusing the cached dependencies)
-- Run `docker build -t ocr_server .`
-
-
-### From PyPI
-
-Run the command
-
-- `pip install django-ocr_translate`
-
-By default torch 2.x will come in its CUDA enabled version. While this works also for CPU, it will also install ~1 GB of cuda dependencies.
-If you wish to run on CPU only, download the file [requirements-torch-cpu.txt](requirements-torch-cpu.txt) first and run
-
-- `pip install -r requirements-torch-cpu.txt`
-
-before installing the python package.
-
-## Running the server
-
-By default the server will use a sqlite database named *db.sqlite3* inside the project main directory.
-If you plan to use a different database, you can either:
-
-- manually edit the [settings.py](mysite/settings.py)
-- Use the provided [Environment variables](#environment-variables)
-See below for a [list of supported databases](#supported-databases)
-
-You will also have to modify the `ALLOWED_HOSTS` in case you plan to access the server from somewhere other than *localhost*.
-
-### From Github installation
-
-The Github repo provides not only the Django app files, but also the already configured project files used to start the server.
-
-Create/Initialize your database by running
-
-- `python manage.py migrate`
-
-inside your project folder.
-
-Run the server using for example one of the following options:
-
-- Django development server. This is more oriented for developing than deploying, but is fine for a self-hosted single-user server accepting connections only on *localhost*
-  - From inside the project directory: `python manage.py runserver PORT`
-  - The suggested PORT would be 4000 as it is the one set by default in the extension
-- [Nginx](https://www.nginx.com/) + [Gunicorn](https://gunicorn.org/):
-  - Check the [Dockerfile](Dockerfile), as this is what the provided image makes use of.
-
-At least for the first time, it is suggested to run the server with the [Environment variables](#environment-variables) `AUTOCREATE_LANGUAGES` and `AUTOCREATE_VALIDATED_MODELS` set to `"true"` to automatically load the validated languages and models provided by the project.
-
-Notes:
-
-- Gunicorn workers will each spawn a separate instance of the loaded models, each taking its own space in the memory. This can quickly fill up the memory especially if running on GPU. Ideally set this to 1.
-- Django development server will spawn new threads for handling incoming requests (if no currently existing thread is free), which share the same memory. Running more than one worker per loaded model concurrently might slow down the actual computation and in some case also block the execution.
-
-### From PyPI installation
-
-When installing the project from PyPI, only the app is available.
-This will need to be integrated in a Django project in order to be used.
-These are the minimal instruction for creating a project and start running the server:
-
-- Run `django-admin startproject mysite` to create a django project
-- Configure the server by replacing the automatically created files (strongly recommended):
-  - [settings.py](mysite/settings.py) with the one available on the repo.
-  - [urls.py](mysite/urls.py) with the one available on the repo.
-- or by manually editing the files:
-  - settings.py: Add the `ocr_translated` app to the `INSTALLED_APPS`
-  - urls.py: Include the `'ocr_translate.urls'` into your project urls.
-- From here follow the same instructions as when starting [from Github](#from-github)
-
-### From docker
-
-This section assumes you have docker installed and the image of the project.
-
-Run the command:
-
-- `docker run --name CONTAINER_NAME -v PATH_TO_YOUR_MODEL_DIRECTORY:/models -v PATH_TO_DIR_WITH_SQLITE_FILE:/data --env-file=PATH_TO_AND_ENV_VARIABLE_FILE -p SERVER_PORT:4000 -d ocr_server`
-
-See the [Environment variables](#environment-variables) section for configuring your environment variable file. Additionaly the docker image defines 2 other variable to automatically create an admin user for managing the database via the django-admin interface:
-
-- `UID`: UID of the user owning the files in /models and /data
-- `GID`: GID of the user owning the files in /models and /data
-- `NUM_WEB_WORKERS`: Number of gunicorn workers for the server
-- `DJANGO_SUPERUSER_USERNAME`: The username of the admin user to be created.
-- `DJANGO_SUPERUSER_PASSWORD`: The password of the admin user to be created.
-
-## Supported Box OCR models
-
-- [EasyOCR](https://github.com/JaidedAI/EasyOCR)
-
-## Supported text OCR models
-
-- Hugging Face [Transformers](https://huggingface.co/docs/transformers/index) VisionEncoderDecoder models
-- [Tesseract](https://github.com/tesseract-ocr/tesseract) (Requires tesseract to be [installed on the machine](https://tesseract-ocr.github.io/tessdoc/Installation.html))
-
-## Supported translation models
-
-- Hugging Face [Seq2Seq](https://huggingface.co/learn/nlp-course/chapter1/7) models
-
-## Endpoints
-
-This is not a REST API. As of now the communication between the server and a front-end is stateful and depend on the languages and models currently loaded on the server.
-In the future it would be interesting to separate the worker and database server, for an actual deployment, but might make the self-hosting more difficult to manage.
-
-| Endpoint | Method | Usage |
-| --- | --- | ---|
-| `/` | GET | Handshake: the server will replay with a JSON response containing information about the available languages/models and the currently in use src/dst language and box/ocr/tsl models |
-| `/get_trans/` | GET | Request to get all the available translations (e.g. using different models) of the text specified by the `text` GET parameter |
-| `/set_lang` | POST | JSON request to switch the currently selected languages to the one specified by the keys: `lang_src`, `lang_dst` |
-| `/set_models` | POST | JSON request to switch the currently loaded models to the one specified by the keys: `box_model_id`, `ocr_model_id`, `tsl_model_id` |
-| `/run_tsl` | POST | JSON request to run the translation for the text specified by the key `text` |
-| `/run_ocrtsl` | POST | JSON request to run the OCR and translation of an image (base64 as the `contents` key) or provide a previously obtained result (md5 of the base64 as the `md5` key). `md5` should be always specified, `contents` is optional |
-
-## Environment variables
-
-The first section of variable is defined at the APP level and will be available both for installation from Github or PyPI.
-The second section of variables is defined at the project level and is only available if using the [settings.py](mysite/settings.py) provided in the repo.
-
-### App variables
-
-| Variable | Values | Usage |
-| --- | --- | --- |
-| `LOAD_ON_START`| false[/true] | Will automatically load the most used source/destination languages and most used models for that language combination at server start|
-| `AUTOCREATE_LANGUAGES` | false[/true] | Will automatically create the Language entries in the database as defined in [languages.json](ocr_translate/OCR_TSL/languages.json) |
-| `AUTOCREATE_VALIDATED_MODELS` | false[/true] | Will automatically create the model entries that have been tested and defined in [models.json](ocr_translate/OCR_TSL/models.json). NOTE: Creation of the models requires the involved languages to already exist in the database |
-| `DEVICE` | cpu[/cuda] | Which device to use with torch |
-| `EASYOCR_MODULE_PATH` | `$HOME/.EasyOCR` | Directory where EasyOCR store its downloaded models |
-| `TRANSFORMERS_CACHE` | `$HOME/.cache/huggingface/hub/` | Directory where [Hugging Face](https://huggingface.co/) models are being stored (either downloaded manually or downloaded by `transformers`) |
-| `TRANSFORMERS_OFFLINE` | 1[/0] | By default `transformers` will try to download missing models. Set this to 0 to only work in offline mode |
-| `TESSERACT_PREFIX` | `$TRANSFORMERS_CACHE/tesseract` | Directory where tesseract will store and look for models |
-| `TESSERACT_ALLOW_DOWNLOAD` | false[/true] | Control whether the app should download missing models (true) or work in offline mode only (false) |
-| `NUM_MAIN_WORKERS` | 4 | Number of `WorkerMessageQueue` workers handling incoming OCR_TSL post requests |
-| `NUM_BOX_WORKERS` | 1 | Number of `WorkerMessageQueue` workers handling box_ocr pipelines (Should be set as 1 until the pipeline is build to handle multiple concurrent request efficiently without slowdowns) |
-| `NUM_OCR_WORKERS` | 1 | Number of `WorkerMessageQueue` workers handling ocr pipelines (Should be set as 1 until the pipeline is build to handle multiple concurrent request efficiently without slowdowns) |
-| `NUM_TSL_WORKERS` | 1 | Number of `WorkerMessageQueue` workers handling translation pipelines (Should be set as 1 until the pipeline is build to handle multiple concurrent request efficiently without slowdowns) |
-
-### Project/server variables
-
-| Variable | Values | Usage |
-| ---- | ---- | ---- |
-| `DJANGO_DEBUG` | false[/true] | Whether to run the server in debug (true) or production (false) mode |
-| `DJANGO_LOG_LEVEL` | INFO | python `logging` level for  |
-| `DATABASE_NAME` | *db.sqlite3* | For `sqlite3` this is the path to the database file. For other backend it should be the name of the database |
-| `DATABASE_ENGINE` | `django.db.backends.sqlite3` | Change this to either a Django or 3rd party provided backend to use another Database type |
-| `DATABASE_HOST` | optional | Required if using another db back-end |
-| `DATABASE_PORT` | optional | Required if using another db back-end |
-| `DATABASE_USER` | optional | Probably required if using another db back-end |
-| `DATABASE_PASSWORD` | optional | Probably required if using another db back-end |
-
-## Supported databases
-
-- [SQLite](https://www.sqlite.org/index.html) This is mostly fine for a self-hosted server accessed by a single  or few users (and it's probably gonna be faster than any other database not running on the same network as the server because of latency).
-- [Postgresql](https://www.postgresql.org/)
-- [MySQL](https://www.mysql.com)/[MariaDB](https://mariadb.org/)
+# OCR_translate
+
+This is a Django app for creating back-end server aimed at performing OCR and translation of images received via a POST request.
+
+The OCR and translation is performed using freely available machine learning models and packages (see below for what is currently implemented).
+
+The server is designed to be used together with [this browser extension](https://github.com/Crivella/ocr_extension), acting as a front-end providing the images and controlling the model languages and models being used.
+
+## Installation
+
+It is strongly suggested to install this project using a [virtual environment](https://docs.python.org/3/library/venv.html).
+
+### From Github
+
+- Clone or download the repository
+  - `git clone https://github.com/Crivella/ocr_translate.git`
+- Install the project dependencies (choose the appropriate files depending if you wanna run on GPU or CPU only):
+  - `pip install -r requirements-torch-[cpu/cuda].txt`
+  - `pip install -r requirements.txt`
+
+### From Docker
+Plan to add a CPU and a CUDA specific image to DockerHUB.
+For now you can create the image yourself by:
+
+- Create a .pip-cache-cpu directory inside your project.
+- Optional: re-install the project dependencies pointing this as the cache folder for pip (will make the build process much faster, by reusing the cached dependencies)
+- Run `docker build -t ocr_server .`
+
+
+### From PyPI
+
+Run the command
+
+- `pip install django-ocr_translate`
+
+By default torch 2.x will come in its CUDA enabled version. While this works also for CPU, it will also install ~1 GB of cuda dependencies.
+If you wish to run on CPU only, download the file [requirements-torch-cpu.txt](requirements-torch-cpu.txt) first and run
+
+- `pip install -r requirements-torch-cpu.txt`
+
+before installing the python package.
+
+## Running the server
+
+By default the server will use a sqlite database named *db.sqlite3* inside the project main directory.
+If you plan to use a different database, you can either:
+
+- manually edit the [settings.py](mysite/settings.py)
+- Use the provided [Environment variables](#environment-variables)
+See below for a [list of supported databases](#supported-databases)
+
+You will also have to modify the `ALLOWED_HOSTS` in case you plan to access the server from somewhere other than *localhost*.
+
+### From Release file
+
+(Tested on Windows 11)
+From the github releases you can download either:
+
+- The [CPU only version](/releases/latest/download/run_server-cpu.exe)
+- The GPU version split in [file 1](/releases/latest/download/run_server-gpu.zip.001) and [file 2](/releases/latest/download/run_server-gpu.zip.002) (The CUDA dependencies makes it take much more space), wich can be restored using tools like [7zip](https://www.7-zip.org/https://www.7-zip.org/) and [NanaZip](https://github.com/M2Team/NanaZip).
+
+Not that every time you run the EXE, it will decompress itself into a temporary folder so:
+
+- The exe will appear as an empty console until all the file are extracted and the actual script start running.
+- By launching the server multiple times without restarting (especially the GPU one), you risk quickly filling up your drive
+
+You can either just start the server and it will run with sensible defaults. Most notably the models files and database will be downloaded/created under `%userprofile%/.ocr_translate`.
+Also the gpu version will attempt to run on GPU by default, and fall-back to CPU if the former is not available.
+
+For customization, you can set the [environment variable](#environment-variables) yourself, either via powershell or by searching for *environment variable* in the settings menu
+
+### From Github installation
+
+The Github repo provides not only the Django app files, but also the already configured project files used to start the server.
+
+Create/Initialize your database by running
+
+- `python manage.py migrate`
+
+inside your project folder.
+
+Run the server using for example one of the following options:
+
+- Django development server. This is more oriented for developing than deploying, but is fine for a self-hosted single-user server accepting connections only on *localhost*
+  - From inside the project directory: `python manage.py runserver PORT`
+  - The suggested PORT would be 4000 as it is the one set by default in the extension
+- [Nginx](https://www.nginx.com/) + [Gunicorn](https://gunicorn.org/):
+  - Check the [Dockerfile](Dockerfile), as this is what the provided image makes use of.
+
+At least for the first time, it is suggested to run the server with the [Environment variables](#environment-variables) `AUTOCREATE_LANGUAGES` and `AUTOCREATE_VALIDATED_MODELS` set to `"true"` to automatically load the validated languages and models provided by the project.
+
+Notes:
+
+- Gunicorn workers will each spawn a separate instance of the loaded models, each taking its own space in the memory. This can quickly fill up the memory especially if running on GPU. Ideally set this to 1.
+- Django development server will spawn new threads for handling incoming requests (if no currently existing thread is free), which share the same memory. Running more than one worker per loaded model concurrently might slow down the actual computation and in some case also block the execution.
+
+### From PyPI installation
+
+When installing the project from PyPI, only the app is available.
+This will need to be integrated in a Django project in order to be used.
+These are the minimal instruction for creating a project and start running the server:
+
+- Run `django-admin startproject mysite` to create a django project
+- Configure the server by replacing the automatically created files (strongly recommended):
+  - [settings.py](mysite/settings.py) with the one available on the repo.
+  - [urls.py](mysite/urls.py) with the one available on the repo.
+- or by manually editing the files:
+  - settings.py: Add the `ocr_translated` app to the `INSTALLED_APPS`
+  - urls.py: Include the `'ocr_translate.urls'` into your project urls.
+- From here follow the same instructions as when starting [from Github](#from-github)
+
+### From docker
+
+This section assumes you have docker installed and the image of the project.
+
+Run the command:
+
+- `docker run --name CONTAINER_NAME -v PATH_TO_YOUR_MODEL_DIRECTORY:/models -v PATH_TO_DIR_WITH_SQLITE_FILE:/data --env-file=PATH_TO_AND_ENV_VARIABLE_FILE -p SERVER_PORT:4000 -d ocr_server`
+
+See the [Environment variables](#environment-variables) section for configuring your environment variable file. Additionaly the docker image defines 2 other variable to automatically create an admin user for managing the database via the django-admin interface:
+
+- `UID`: UID of the user owning the files in /models and /data
+- `GID`: GID of the user owning the files in /models and /data
+- `NUM_WEB_WORKERS`: Number of gunicorn workers for the server
+- `DJANGO_SUPERUSER_USERNAME`: The username of the admin user to be created.
+- `DJANGO_SUPERUSER_PASSWORD`: The password of the admin user to be created.
+
+## Supported Box OCR models
+
+- [EasyOCR](https://github.com/JaidedAI/EasyOCR)
+
+## Supported text OCR models
+
+- Hugging Face [Transformers](https://huggingface.co/docs/transformers/index) VisionEncoderDecoder models
+- [Tesseract](https://github.com/tesseract-ocr/tesseract) (Requires tesseract to be [installed on the machine](https://tesseract-ocr.github.io/tessdoc/Installation.html))
+
+## Supported translation models
+
+- Hugging Face [Seq2Seq](https://huggingface.co/learn/nlp-course/chapter1/7) models
+
+## Endpoints
+
+This is not a REST API. As of now the communication between the server and a front-end is stateful and depend on the languages and models currently loaded on the server.
+In the future it would be interesting to separate the worker and database server, for an actual deployment, but might make the self-hosting more difficult to manage.
+
+| Endpoint | Method | Usage |
+| --- | --- | ---|
+| `/` | GET | Handshake: the server will replay with a JSON response containing information about the available languages/models and the currently in use src/dst language and box/ocr/tsl models |
+| `/get_trans/` | GET | Request to get all the available translations (e.g. using different models) of the text specified by the `text` GET parameter |
+| `/set_lang` | POST | JSON request to switch the currently selected languages to the one specified by the keys: `lang_src`, `lang_dst` |
+| `/set_models` | POST | JSON request to switch the currently loaded models to the one specified by the keys: `box_model_id`, `ocr_model_id`, `tsl_model_id` |
+| `/run_tsl` | POST | JSON request to run the translation for the text specified by the key `text` |
+| `/run_ocrtsl` | POST | JSON request to run the OCR and translation of an image (base64 as the `contents` key) or provide a previously obtained result (md5 of the base64 as the `md5` key). `md5` should be always specified, `contents` is optional |
+
+## Environment variables
+
+The first section of variable is defined at the APP level and will be available both for installation from Github or PyPI.
+The second section of variables is defined at the project level and is only available if using the [settings.py](mysite/settings.py) provided in the repo.
+
+### App variables
+
+| Variable | Values | Usage |
+| --- | --- | --- |
+| `LOAD_ON_START`| false[/true] | Will automatically load the most used source/destination languages and most used models for that language combination at server start|
+| `AUTOCREATE_LANGUAGES` | false[/true] | Will automatically create the Language entries in the database as defined in [languages.json](ocr_translate/OCR_TSL/languages.json) |
+| `AUTOCREATE_VALIDATED_MODELS` | false[/true] | Will automatically create the model entries that have been tested and defined in [models.json](ocr_translate/OCR_TSL/models.json). NOTE: Creation of the models requires the involved languages to already exist in the database |
+| `DEVICE` | cpu[/cuda] | Which device to use with torch |
+| `EASYOCR_MODULE_PATH` | `$HOME/.EasyOCR` | Directory where EasyOCR store its downloaded models |
+| `TRANSFORMERS_CACHE` | `$HOME/.cache/huggingface/hub/` | Directory where [Hugging Face](https://huggingface.co/) models are being stored (either downloaded manually or downloaded by `transformers`) |
+| `TRANSFORMERS_OFFLINE` | 1[/0] | By default `transformers` will try to download missing models. Set this to 0 to only work in offline mode |
+| `TESSERACT_PREFIX` | `$TRANSFORMERS_CACHE/tesseract` | Directory where tesseract will store and look for models |
+| `TESSERACT_ALLOW_DOWNLOAD` | false[/true] | Control whether the app should download missing models (true) or work in offline mode only (false) |
+| `NUM_MAIN_WORKERS` | 4 | Number of `WorkerMessageQueue` workers handling incoming OCR_TSL post requests |
+| `NUM_BOX_WORKERS` | 1 | Number of `WorkerMessageQueue` workers handling box_ocr pipelines (Should be set as 1 until the pipeline is build to handle multiple concurrent request efficiently without slowdowns) |
+| `NUM_OCR_WORKERS` | 1 | Number of `WorkerMessageQueue` workers handling ocr pipelines (Should be set as 1 until the pipeline is build to handle multiple concurrent request efficiently without slowdowns) |
+| `NUM_TSL_WORKERS` | 1 | Number of `WorkerMessageQueue` workers handling translation pipelines (Should be set as 1 until the pipeline is build to handle multiple concurrent request efficiently without slowdowns) |
+
+### Project/server variables
+
+| Variable | Values | Usage |
+| ---- | ---- | ---- |
+| `DJANGO_DEBUG` | false[/true] | Whether to run the server in debug (true) or production (false) mode |
+| `DJANGO_LOG_LEVEL` | INFO | python `logging` level for  |
+| `DATABASE_NAME` | *db.sqlite3* | For `sqlite3` this is the path to the database file. For other backend it should be the name of the database |
+| `DATABASE_ENGINE` | `django.db.backends.sqlite3` | Change this to either a Django or 3rd party provided backend to use another Database type |
+| `DATABASE_HOST` | optional | Required if using another db back-end |
+| `DATABASE_PORT` | optional | Required if using another db back-end |
+| `DATABASE_USER` | optional | Probably required if using another db back-end |
+| `DATABASE_PASSWORD` | optional | Probably required if using another db back-end |
+
+## Supported databases
+
+- [SQLite](https://www.sqlite.org/index.html) This is mostly fine for a self-hosted server accessed by a single  or few users (and it's probably gonna be faster than any other database not running on the same network as the server because of latency).
+- [Postgresql](https://www.postgresql.org/)
+- [MySQL](https://www.mysql.com)/[MariaDB](https://mariadb.org/)
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/base.py` & `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/initializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,117 @@
-###################################################################################
-# ocr_translate - a django app to perform OCR and translation of images.          #
-# Copyright (C) 2023-present Davide Grassano                                      #
-#                                                                                 #
-# This program is free software: you can redistribute it and/or modify            #
-# it under the terms of the GNU General Public License as published by            #
-# the Free Software Foundation, either version 3 of the License.                  #
-#                                                                                 #
-# This program is distributed in the hope that it will be useful,                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
-# GNU General Public License for more details.                                    #
-#                                                                                 #
-# You should have received a copy of the GNU General Public License               #
-# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
-#                                                                                 #
-# Home: https://github.com/Crivella/ocr_translate                                 #
-###################################################################################
-import json
-import logging
-import os
-from pathlib import Path
-
-from transformers import (AutoImageProcessor, AutoModel, AutoModelForSeq2SeqLM,
-                          AutoTokenizer, VisionEncoderDecoderModel)
-
-from .. import models as m
-
-logger = logging.getLogger('ocr.general')
-
-root = Path(os.environ.get('TRANSFORMERS_CACHE', '.'))
-logger.debug(f'Cache dir: {root}')
-dev = os.environ.get('DEVICE', 'cpu')
-
-def load(loader, model_id: str):
-    res = None
-    try:
-        mid = root / model_id
-        logger.debug(f'Attempt loading from store: "{loader}" "{mid}"')
-        res = loader.from_pretrained(mid)
-    except Exception:
-        # Needed to catch some weird exception from transformers
-        # eg: huggingface_hub.utils._validators.HFValidationError: Repo id must use alphanumeric chars or '-', '_', '.', '--' and '..' are forbidden, '-' and '.' cannot start or end the name, max length is 96: ...
-        logger.debug(f'Attempt loading from cache: "{loader}" "{model_id}" "{root}"')
-        res = loader.from_pretrained(model_id, cache_dir=root)
-    return res
-
-mapping = {
-    'tokenizer': AutoTokenizer,
-    'ved_model': VisionEncoderDecoderModel,
-    'model': AutoModel,
-    'image_processor': AutoImageProcessor,
-    'seq2seq': AutoModelForSeq2SeqLM
-}
-
-accept_device = ['ved_model', 'seq2seq', 'model']
-
-def load_hugginface_model(model_id: str, request: list[str]):
-    res = {}
-    for r in request:
-        if r not in mapping:
-            raise ValueError(f'Unknown request: {r}')
-        v = load(mapping[r], model_id)
-        if v is None:
-            raise ValueError(f'Could not load model: {model_id}')
-        
-        if r in accept_device:
-            v = v.to(dev)
-
-        res[r] = v
-
-    return res
-
-if os.environ.get('AUTOCREATE_LANGUAGES', 'false').lower() == 'true':
-    cwd = Path(__file__).parent
-    with open(cwd / 'languages.json', encoding='utf-8') as f:
-        langs = json.load(f)
-
-    for lang in langs:
-        logger.debug(f'Creating language: {lang}')
-        name = lang.pop('name')
-        iso1 = lang.pop('iso1')
-        iso2t = lang.pop('iso2t')
-        iso2b = lang.pop('iso2b')
-        iso3 = lang.pop('iso3')
-        l, _ = m.Language.objects.get_or_create(name=name, iso1=iso1, iso2t=iso2t, iso2b=iso2b, iso3=iso3)
-        for k,v in lang.items():
-            setattr(l, k, v)
-        l.save()
-
-if os.environ.get('AUTOCREATE_VALIDATED_MODELS', 'false').lower() == 'true':
-    cwd = Path(__file__).parent
-    with open(cwd / 'models.json') as f:
-        models = json.load(f)
-
-    for box in models['box']:
-        logger.debug(f'Creating box model: {box}')
-        lang = box.pop('lang')
-        lcode = box.pop('lang_code')
-        model, _ = m.OCRBoxModel.objects.get_or_create(**box)
-        model.language_format = lcode
-        for l in lang:
-            model.languages.add(m.Language.objects.get(iso1=l))
-        model.save()
-
-    for ocr in models['ocr']:
-        logger.debug(f'Creating ocr model: {ocr}')
-        lang = ocr.pop('lang')
-        lcode = ocr.pop('lang_code')
-        model, _ = m.OCRModel.objects.get_or_create(**ocr)
-        model.language_format = lcode
-        for l in lang:
-            model.languages.add(m.Language.objects.get(iso1=l))
-        model.save()
-
-    for tsl in models['tsl']:
-        logger.debug(f'Creating tsl model: {tsl}')
-        src = tsl.pop('lang_src')
-        dst = tsl.pop('lang_dst')
-        lcode = tsl.pop('lang_code', None)
-        model, _ = m.TSLModel.objects.get_or_create(**tsl)
-        model.language_format = lcode
-        for l in src:
-            logger.debug(f'Adding src language: {l}')
-            kw = {lcode: l}
-            model.src_languages.add(*m.Language.objects.filter(**kw))
-
-        for l in dst:
-            logger.debug(f'Adding dst language: {l}')
-            kw = {lcode: l}
-            model.dst_languages.add(*m.Language.objects.filter(**kw))
-        model.save()
-
-    base_option, _ = m.OptionDict.objects.get_or_create(options={})
+###################################################################################
+# ocr_translate - a django app to perform OCR and translation of images.          #
+# Copyright (C) 2023-present Davide Grassano                                      #
+#                                                                                 #
+# This program is free software: you can redistribute it and/or modify            #
+# it under the terms of the GNU General Public License as published by            #
+# the Free Software Foundation, either version 3 of the License.                  #
+#                                                                                 #
+# This program is distributed in the hope that it will be useful,                 #
+# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
+# GNU General Public License for more details.                                    #
+#                                                                                 #
+# You should have received a copy of the GNU General Public License               #
+# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
+#                                                                                 #
+# Home: https://github.com/Crivella/ocr_translate                                 #
+###################################################################################
+"""Initialize the server based on environment variables."""
+import json
+import logging
+from pathlib import Path
+
+from django.db.models import Count
+
+from .. import models as m
+from .box import load_box_model
+from .lang import load_lang_dst, load_lang_src
+from .ocr import load_ocr_model
+from .tsl import load_tsl_model
+
+logger = logging.getLogger('ocr.general')
+
+def init_most_used():
+    """Initialize the server with the most used languages and models."""
+    src = m.Language.objects.annotate(count=Count('trans_src')).order_by('-count').first()
+    dst = m.Language.objects.annotate(count=Count('trans_dst')).order_by('-count').first()
+
+    if src:
+        load_lang_src(src.iso1)
+    if dst:
+        load_lang_dst(dst.iso1)
+
+    box = m.OCRBoxModel.objects.annotate(count=Count('box_runs')).order_by('-count').first()
+    ocr = m.OCRModel.objects.annotate(count=Count('ocr_runs')).order_by('-count').first()
+    tsl = m.TSLModel.objects.annotate(count=Count('tsl_runs')).order_by('-count').first()
+
+    if box:
+        load_box_model(box.name)
+    if ocr:
+        load_ocr_model(ocr.name)
+    if tsl:
+        load_tsl_model(tsl.name)
+
+def auto_create_languages():
+    """Create Language objects from json file."""
+    cwd = Path(__file__).parent
+    with open(cwd / 'languages.json', encoding='utf-8') as f:
+        langs = json.load(f)
+
+    for lang in langs:
+        logger.debug(f'Creating language: {lang}')
+        name = lang.pop('name')
+        iso1 = lang.pop('iso1')
+        iso2t = lang.pop('iso2t')
+        iso2b = lang.pop('iso2b')
+        iso3 = lang.pop('iso3')
+        l, _ = m.Language.objects.get_or_create(name=name, iso1=iso1, iso2t=iso2t, iso2b=iso2b, iso3=iso3)
+        for k,v in lang.items():
+            setattr(l, k, v)
+        l.save()
+
+def auto_create_models():
+    """Create OCR and TSL models from json file. Also create default OptionDict"""
+    cwd = Path(__file__).parent
+    with open(cwd / 'models.json', encoding='utf-8') as f:
+        models = json.load(f)
+
+    for box in models['box']:
+        logger.debug(f'Creating box model: {box}')
+        lang = box.pop('lang')
+        lcode = box.pop('lang_code')
+        model, _ = m.OCRBoxModel.objects.get_or_create(**box)
+        model.language_format = lcode
+        for l in lang:
+            model.languages.add(m.Language.objects.get(iso1=l))
+        model.save()
+
+    for ocr in models['ocr']:
+        logger.debug(f'Creating ocr model: {ocr}')
+        lang = ocr.pop('lang')
+        lcode = ocr.pop('lang_code')
+        model, _ = m.OCRModel.objects.get_or_create(**ocr)
+        model.language_format = lcode
+        for l in lang:
+            model.languages.add(m.Language.objects.get(iso1=l))
+        model.save()
+
+    for tsl in models['tsl']:
+        logger.debug(f'Creating tsl model: {tsl}')
+        src = tsl.pop('lang_src')
+        dst = tsl.pop('lang_dst')
+        lcode = tsl.pop('lang_code', None)
+        model, _ = m.TSLModel.objects.get_or_create(**tsl)
+        model.language_format = lcode
+        for l in src:
+            logger.debug(f'Adding src language: {l}')
+            kwargs = {lcode: l}
+            model.src_languages.add(*m.Language.objects.filter(**kwargs))
+
+        for l in dst:
+            logger.debug(f'Adding dst language: {l}')
+            kwargs = {lcode: l}
+            model.dst_languages.add(*m.Language.objects.filter(**kwargs))
+        model.save()
+
+    m.OptionDict.objects.get_or_create(options={})
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/models.json` & `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/models.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 18% similar despite different names*

```diff
@@ -1,217 +1,221 @@
-00000000: 7b0a 2020 2020 2262 6f78 223a 205b 0a20  {.    "box": [. 
-00000010: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00000020: 2020 2020 2022 6e61 6d65 223a 2022 6561       "name": "ea
-00000030: 7379 6f63 7222 2c0a 2020 2020 2020 2020  syocr",.        
-00000040: 2020 2020 226c 616e 6722 3a20 5b22 656e      "lang": ["en
-00000050: 222c 2022 6a61 222c 2022 7a68 222c 2022  ", "ja", "zh", "
-00000060: 6b6f 225d 2c0a 2020 2020 2020 2020 2020  ko"],.          
-00000070: 2020 226c 616e 675f 636f 6465 223a 2022    "lang_code": "
-00000080: 6561 7379 6f63 7222 0a20 2020 2020 2020  easyocr".       
-00000090: 207d 0a20 2020 205d 2c0a 2020 2020 226f   }.    ],.    "o
-000000a0: 6372 223a 205b 0a20 2020 2020 2020 207b  cr": [.        {
-000000b0: 0a20 2020 2020 2020 2020 2020 2022 6e61  .            "na
-000000c0: 6d65 223a 2022 6b68 612d 7768 6974 652f  me": "kha-white/
-000000d0: 6d61 6e67 612d 6f63 722d 6261 7365 222c  manga-ocr-base",
-000000e0: 0a20 2020 2020 2020 2020 2020 2022 6c61  .            "la
-000000f0: 6e67 223a 205b 226a 6122 5d2c 0a20 2020  ng": ["ja"],.   
-00000100: 2020 2020 2020 2020 2022 6c61 6e67 5f63           "lang_c
-00000110: 6f64 6522 3a20 2269 736f 3122 0a20 2020  ode": "iso1".   
-00000120: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00000130: 7b0a 2020 2020 2020 2020 2020 2020 226e  {.            "n
-00000140: 616d 6522 3a20 2274 6573 7365 7261 6374  ame": "tesseract
-00000150: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000160: 6c61 6e67 223a 205b 2265 6e22 2c20 226a  lang": ["en", "j
-00000170: 6122 2c20 227a 6822 2c20 226b 6f22 5d2c  a", "zh", "ko"],
-00000180: 0a20 2020 2020 2020 2020 2020 2022 6c61  .            "la
-00000190: 6e67 5f63 6f64 6522 3a20 2274 6573 7365  ng_code": "tesse
-000001a0: 7261 6374 220a 2020 2020 2020 2020 7d0a  ract".        }.
-000001b0: 2020 2020 5d2c 0a20 2020 2022 7473 6c22      ],.    "tsl"
-000001c0: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-000001d0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-000001e0: 3a20 2248 656c 7369 6e6b 692d 4e4c 502f  : "Helsinki-NLP/
-000001f0: 6f70 7573 2d6d 742d 7a68 2d65 6e22 2c0a  opus-mt-zh-en",.
-00000200: 2020 2020 2020 2020 2020 2020 226c 616e              "lan
-00000210: 675f 7372 6322 3a20 5b22 7a68 225d 2c0a  g_src": ["zh"],.
-00000220: 2020 2020 2020 2020 2020 2020 226c 616e              "lan
-00000230: 675f 6473 7422 3a20 5b22 656e 225d 2c0a  g_dst": ["en"],.
-00000240: 2020 2020 2020 2020 2020 2020 226c 616e              "lan
-00000250: 675f 636f 6465 223a 2022 6973 6f31 220a  g_code": "iso1".
-00000260: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000270: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00000280: 2022 6e61 6d65 223a 2022 4865 6c73 696e   "name": "Helsin
-00000290: 6b69 2d4e 4c50 2f6f 7075 732d 6d74 2d6a  ki-NLP/opus-mt-j
-000002a0: 612d 656e 222c 0a20 2020 2020 2020 2020  a-en",.         
-000002b0: 2020 2022 6c61 6e67 5f73 7263 223a 205b     "lang_src": [
-000002c0: 226a 6122 5d2c 0a20 2020 2020 2020 2020  "ja"],.         
-000002d0: 2020 2022 6c61 6e67 5f64 7374 223a 205b     "lang_dst": [
-000002e0: 2265 6e22 5d2c 0a20 2020 2020 2020 2020  "en"],.         
-000002f0: 2020 2022 6c61 6e67 5f63 6f64 6522 3a20     "lang_code": 
-00000300: 2269 736f 3122 0a20 2020 2020 2020 207d  "iso1".        }
-00000310: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
-00000320: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-00000330: 2273 7461 6b61 2f66 7567 756d 742d 6a61  "staka/fugumt-ja
-00000340: 2d65 6e22 2c0a 2020 2020 2020 2020 2020  -en",.          
-00000350: 2020 226c 616e 675f 7372 6322 3a20 5b22    "lang_src": ["
-00000360: 6a61 225d 2c0a 2020 2020 2020 2020 2020  ja"],.          
-00000370: 2020 226c 616e 675f 6473 7422 3a20 5b22    "lang_dst": ["
-00000380: 656e 225d 2c0a 2020 2020 2020 2020 2020  en"],.          
-00000390: 2020 226c 616e 675f 636f 6465 223a 2022    "lang_code": "
-000003a0: 6973 6f31 220a 2020 2020 2020 2020 7d2c  iso1".        },
-000003b0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-000003c0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-000003d0: 4865 6c73 696e 6b69 2d4e 4c50 2f6f 7075  Helsinki-NLP/opu
-000003e0: 732d 6d74 2d6b 6f2d 656e 222c 0a20 2020  s-mt-ko-en",.   
-000003f0: 2020 2020 2020 2020 2022 6c61 6e67 5f73           "lang_s
-00000400: 7263 223a 205b 226b 6f22 5d2c 0a20 2020  rc": ["ko"],.   
-00000410: 2020 2020 2020 2020 2022 6c61 6e67 5f64           "lang_d
-00000420: 7374 223a 205b 2265 6e22 5d2c 0a20 2020  st": ["en"],.   
-00000430: 2020 2020 2020 2020 2022 6c61 6e67 5f63           "lang_c
-00000440: 6f64 6522 3a20 2269 736f 3122 0a20 2020  ode": "iso1".   
-00000450: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00000460: 7b0a 2020 2020 2020 2020 2020 2020 226e  {.            "n
-00000470: 616d 6522 3a20 2266 6163 6562 6f6f 6b2f  ame": "facebook/
-00000480: 6d32 6d31 3030 5f34 3138 4d22 2c0a 2020  m2m100_418M",.  
-00000490: 2020 2020 2020 2020 2020 226c 616e 675f            "lang_
-000004a0: 7372 6322 3a20 5b22 6166 222c 2022 616d  src": ["af", "am
-000004b0: 222c 2022 6172 222c 2022 617a 222c 2022  ", "ar", "az", "
-000004c0: 6261 222c 2022 6265 222c 2022 6267 222c  ba", "be", "bg",
-000004d0: 2022 626e 222c 2022 6272 222c 2022 6273   "bn", "br", "bs
-000004e0: 222c 2022 6373 222c 2022 6379 222c 2022  ", "cs", "cy", "
-000004f0: 6461 222c 2022 6465 222c 2022 656e 222c  da", "de", "en",
-00000500: 2022 6574 222c 2022 6661 222c 2022 6666   "et", "fa", "ff
-00000510: 222c 2022 6669 222c 2022 6672 222c 2022  ", "fi", "fr", "
-00000520: 6679 222c 2022 6761 222c 2022 676c 222c  fy", "ga", "gl",
-00000530: 2022 6775 222c 2022 6861 222c 2022 6865   "gu", "ha", "he
-00000540: 222c 2022 6869 222c 2022 6872 222c 2022  ", "hi", "hr", "
-00000550: 6875 222c 2022 6879 222c 2022 6964 222c  hu", "hy", "id",
-00000560: 2022 6967 222c 2022 6973 222c 2022 6974   "ig", "is", "it
-00000570: 222c 2022 6a61 222c 2022 6a76 222c 2022  ", "ja", "jv", "
-00000580: 6b61 222c 2022 6b6b 222c 2022 6b6d 222c  ka", "kk", "km",
-00000590: 2022 6b6e 222c 2022 6b6f 222c 2022 6c67   "kn", "ko", "lg
-000005a0: 222c 2022 6c6e 222c 2022 6c6f 222c 2022  ", "ln", "lo", "
-000005b0: 6c74 222c 2022 6c76 222c 2022 6d67 222c  lt", "lv", "mg",
-000005c0: 2022 6d6b 222c 2022 6d6c 222c 2022 6d6e   "mk", "ml", "mn
-000005d0: 222c 2022 6d72 222c 2022 6d73 222c 2022  ", "mr", "ms", "
-000005e0: 6d79 222c 2022 6e65 222c 2022 6e6f 222c  my", "ne", "no",
-000005f0: 2022 6f63 222c 2022 6f72 222c 2022 706c   "oc", "or", "pl
-00000600: 222c 2022 7074 222c 2022 7275 222c 2022  ", "pt", "ru", "
-00000610: 7364 222c 2022 736b 222c 2022 736c 222c  sd", "sk", "sl",
-00000620: 2022 736f 222c 2022 7371 222c 2022 7372   "so", "sq", "sr
-00000630: 222c 2022 7373 222c 2022 7375 222c 2022  ", "ss", "su", "
-00000640: 7376 222c 2022 7377 222c 2022 7461 222c  sv", "sw", "ta",
-00000650: 2022 7468 222c 2022 746c 222c 2022 746e   "th", "tl", "tn
-00000660: 222c 2022 7472 222c 2022 756b 222c 2022  ", "tr", "uk", "
-00000670: 7572 222c 2022 757a 222c 2022 7669 222c  ur", "uz", "vi",
-00000680: 2022 776f 222c 2022 7868 222c 2022 7969   "wo", "xh", "yi
-00000690: 222c 2022 796f 222c 2022 7a68 222c 2022  ", "yo", "zh", "
-000006a0: 7a75 225d 2c0a 2020 2020 2020 2020 2020  zu"],.          
-000006b0: 2020 226c 616e 675f 6473 7422 3a20 5b22    "lang_dst": ["
-000006c0: 6166 222c 2022 616d 222c 2022 6172 222c  af", "am", "ar",
-000006d0: 2022 617a 222c 2022 6261 222c 2022 6265   "az", "ba", "be
-000006e0: 222c 2022 6267 222c 2022 626e 222c 2022  ", "bg", "bn", "
-000006f0: 6272 222c 2022 6273 222c 2022 6373 222c  br", "bs", "cs",
-00000700: 2022 6379 222c 2022 6461 222c 2022 6465   "cy", "da", "de
-00000710: 222c 2022 656e 222c 2022 6574 222c 2022  ", "en", "et", "
-00000720: 6661 222c 2022 6666 222c 2022 6669 222c  fa", "ff", "fi",
-00000730: 2022 6672 222c 2022 6679 222c 2022 6761   "fr", "fy", "ga
-00000740: 222c 2022 676c 222c 2022 6775 222c 2022  ", "gl", "gu", "
-00000750: 6861 222c 2022 6865 222c 2022 6869 222c  ha", "he", "hi",
-00000760: 2022 6872 222c 2022 6875 222c 2022 6879   "hr", "hu", "hy
-00000770: 222c 2022 6964 222c 2022 6967 222c 2022  ", "id", "ig", "
-00000780: 6973 222c 2022 6974 222c 2022 6a61 222c  is", "it", "ja",
-00000790: 2022 6a76 222c 2022 6b61 222c 2022 6b6b   "jv", "ka", "kk
-000007a0: 222c 2022 6b6d 222c 2022 6b6e 222c 2022  ", "km", "kn", "
-000007b0: 6b6f 222c 2022 6c67 222c 2022 6c6e 222c  ko", "lg", "ln",
-000007c0: 2022 6c6f 222c 2022 6c74 222c 2022 6c76   "lo", "lt", "lv
-000007d0: 222c 2022 6d67 222c 2022 6d6b 222c 2022  ", "mg", "mk", "
-000007e0: 6d6c 222c 2022 6d6e 222c 2022 6d72 222c  ml", "mn", "mr",
-000007f0: 2022 6d73 222c 2022 6d79 222c 2022 6e65   "ms", "my", "ne
-00000800: 222c 2022 6e6f 222c 2022 6f63 222c 2022  ", "no", "oc", "
-00000810: 6f72 222c 2022 706c 222c 2022 7074 222c  or", "pl", "pt",
-00000820: 2022 7275 222c 2022 7364 222c 2022 736b   "ru", "sd", "sk
-00000830: 222c 2022 736c 222c 2022 736f 222c 2022  ", "sl", "so", "
-00000840: 7371 222c 2022 7372 222c 2022 7373 222c  sq", "sr", "ss",
-00000850: 2022 7375 222c 2022 7376 222c 2022 7377   "su", "sv", "sw
-00000860: 222c 2022 7461 222c 2022 7468 222c 2022  ", "ta", "th", "
-00000870: 746c 222c 2022 746e 222c 2022 7472 222c  tl", "tn", "tr",
-00000880: 2022 756b 222c 2022 7572 222c 2022 757a   "uk", "ur", "uz
-00000890: 222c 2022 7669 222c 2022 776f 222c 2022  ", "vi", "wo", "
-000008a0: 7868 222c 2022 7969 222c 2022 796f 222c  xh", "yi", "yo",
-000008b0: 2022 7a68 222c 2022 7a75 225d 2c0a 2020   "zh", "zu"],.  
-000008c0: 2020 2020 2020 2020 2020 226c 616e 675f            "lang_
-000008d0: 636f 6465 223a 2022 6661 6365 626f 6f6b  code": "facebook
-000008e0: 4d32 4d22 0a20 2020 2020 2020 207d 2c0a  M2M".        },.
-000008f0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000900: 2020 2020 2020 226e 616d 6522 3a20 2266        "name": "f
-00000910: 6163 6562 6f6f 6b2f 6d32 6d31 3030 5f31  acebook/m2m100_1
-00000920: 2e32 4222 2c0a 2020 2020 2020 2020 2020  .2B",.          
-00000930: 2020 226c 616e 675f 7372 6322 3a20 5b22    "lang_src": ["
-00000940: 6166 222c 2022 616d 222c 2022 6172 222c  af", "am", "ar",
-00000950: 2022 617a 222c 2022 6261 222c 2022 6265   "az", "ba", "be
-00000960: 222c 2022 6267 222c 2022 626e 222c 2022  ", "bg", "bn", "
-00000970: 6272 222c 2022 6273 222c 2022 6373 222c  br", "bs", "cs",
-00000980: 2022 6379 222c 2022 6461 222c 2022 6465   "cy", "da", "de
-00000990: 222c 2022 656e 222c 2022 6574 222c 2022  ", "en", "et", "
-000009a0: 6661 222c 2022 6666 222c 2022 6669 222c  fa", "ff", "fi",
-000009b0: 2022 6672 222c 2022 6679 222c 2022 6761   "fr", "fy", "ga
-000009c0: 222c 2022 676c 222c 2022 6775 222c 2022  ", "gl", "gu", "
-000009d0: 6861 222c 2022 6865 222c 2022 6869 222c  ha", "he", "hi",
-000009e0: 2022 6872 222c 2022 6875 222c 2022 6879   "hr", "hu", "hy
-000009f0: 222c 2022 6964 222c 2022 6967 222c 2022  ", "id", "ig", "
-00000a00: 6973 222c 2022 6974 222c 2022 6a61 222c  is", "it", "ja",
-00000a10: 2022 6a76 222c 2022 6b61 222c 2022 6b6b   "jv", "ka", "kk
-00000a20: 222c 2022 6b6d 222c 2022 6b6e 222c 2022  ", "km", "kn", "
-00000a30: 6b6f 222c 2022 6c67 222c 2022 6c6e 222c  ko", "lg", "ln",
-00000a40: 2022 6c6f 222c 2022 6c74 222c 2022 6c76   "lo", "lt", "lv
-00000a50: 222c 2022 6d67 222c 2022 6d6b 222c 2022  ", "mg", "mk", "
-00000a60: 6d6c 222c 2022 6d6e 222c 2022 6d72 222c  ml", "mn", "mr",
-00000a70: 2022 6d73 222c 2022 6d79 222c 2022 6e65   "ms", "my", "ne
-00000a80: 222c 2022 6e6f 222c 2022 6f63 222c 2022  ", "no", "oc", "
-00000a90: 6f72 222c 2022 706c 222c 2022 7074 222c  or", "pl", "pt",
-00000aa0: 2022 7275 222c 2022 7364 222c 2022 736b   "ru", "sd", "sk
-00000ab0: 222c 2022 736c 222c 2022 736f 222c 2022  ", "sl", "so", "
-00000ac0: 7371 222c 2022 7372 222c 2022 7373 222c  sq", "sr", "ss",
-00000ad0: 2022 7375 222c 2022 7376 222c 2022 7377   "su", "sv", "sw
-00000ae0: 222c 2022 7461 222c 2022 7468 222c 2022  ", "ta", "th", "
-00000af0: 746c 222c 2022 746e 222c 2022 7472 222c  tl", "tn", "tr",
-00000b00: 2022 756b 222c 2022 7572 222c 2022 757a   "uk", "ur", "uz
-00000b10: 222c 2022 7669 222c 2022 776f 222c 2022  ", "vi", "wo", "
-00000b20: 7868 222c 2022 7969 222c 2022 796f 222c  xh", "yi", "yo",
-00000b30: 2022 7a68 222c 2022 7a75 225d 2c0a 2020   "zh", "zu"],.  
-00000b40: 2020 2020 2020 2020 2020 226c 616e 675f            "lang_
-00000b50: 6473 7422 3a20 5b22 6166 222c 2022 616d  dst": ["af", "am
-00000b60: 222c 2022 6172 222c 2022 617a 222c 2022  ", "ar", "az", "
-00000b70: 6261 222c 2022 6265 222c 2022 6267 222c  ba", "be", "bg",
-00000b80: 2022 626e 222c 2022 6272 222c 2022 6273   "bn", "br", "bs
-00000b90: 222c 2022 6373 222c 2022 6379 222c 2022  ", "cs", "cy", "
-00000ba0: 6461 222c 2022 6465 222c 2022 656e 222c  da", "de", "en",
-00000bb0: 2022 6574 222c 2022 6661 222c 2022 6666   "et", "fa", "ff
-00000bc0: 222c 2022 6669 222c 2022 6672 222c 2022  ", "fi", "fr", "
-00000bd0: 6679 222c 2022 6761 222c 2022 676c 222c  fy", "ga", "gl",
-00000be0: 2022 6775 222c 2022 6861 222c 2022 6865   "gu", "ha", "he
-00000bf0: 222c 2022 6869 222c 2022 6872 222c 2022  ", "hi", "hr", "
-00000c00: 6875 222c 2022 6879 222c 2022 6964 222c  hu", "hy", "id",
-00000c10: 2022 6967 222c 2022 6973 222c 2022 6974   "ig", "is", "it
-00000c20: 222c 2022 6a61 222c 2022 6a76 222c 2022  ", "ja", "jv", "
-00000c30: 6b61 222c 2022 6b6b 222c 2022 6b6d 222c  ka", "kk", "km",
-00000c40: 2022 6b6e 222c 2022 6b6f 222c 2022 6c67   "kn", "ko", "lg
-00000c50: 222c 2022 6c6e 222c 2022 6c6f 222c 2022  ", "ln", "lo", "
-00000c60: 6c74 222c 2022 6c76 222c 2022 6d67 222c  lt", "lv", "mg",
-00000c70: 2022 6d6b 222c 2022 6d6c 222c 2022 6d6e   "mk", "ml", "mn
-00000c80: 222c 2022 6d72 222c 2022 6d73 222c 2022  ", "mr", "ms", "
-00000c90: 6d79 222c 2022 6e65 222c 2022 6e6f 222c  my", "ne", "no",
-00000ca0: 2022 6f63 222c 2022 6f72 222c 2022 706c   "oc", "or", "pl
-00000cb0: 222c 2022 7074 222c 2022 7275 222c 2022  ", "pt", "ru", "
-00000cc0: 7364 222c 2022 736b 222c 2022 736c 222c  sd", "sk", "sl",
-00000cd0: 2022 736f 222c 2022 7371 222c 2022 7372   "so", "sq", "sr
-00000ce0: 222c 2022 7373 222c 2022 7375 222c 2022  ", "ss", "su", "
-00000cf0: 7376 222c 2022 7377 222c 2022 7461 222c  sv", "sw", "ta",
-00000d00: 2022 7468 222c 2022 746c 222c 2022 746e   "th", "tl", "tn
-00000d10: 222c 2022 7472 222c 2022 756b 222c 2022  ", "tr", "uk", "
-00000d20: 7572 222c 2022 757a 222c 2022 7669 222c  ur", "uz", "vi",
-00000d30: 2022 776f 222c 2022 7868 222c 2022 7969   "wo", "xh", "yi
-00000d40: 222c 2022 796f 222c 2022 7a68 222c 2022  ", "yo", "zh", "
-00000d50: 7a75 225d 2c0a 2020 2020 2020 2020 2020  zu"],.          
-00000d60: 2020 226c 616e 675f 636f 6465 223a 2022    "lang_code": "
-00000d70: 6661 6365 626f 6f6b 4d32 4d22 0a20 2020  facebookM2M".   
-00000d80: 2020 2020 207d 0a20 2020 205d 0a7d            }.    ].}
+00000000: 7b0d 0a20 2020 2022 626f 7822 3a20 5b0d  {..    "box": [.
+00000010: 0a20 2020 2020 2020 207b 0d0a 2020 2020  .        {..    
+00000020: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00000030: 2265 6173 796f 6372 222c 0d0a 2020 2020  "easyocr",..    
+00000040: 2020 2020 2020 2020 226c 616e 6722 3a20          "lang": 
+00000050: 5b22 656e 222c 2022 6a61 222c 2022 7a68  ["en", "ja", "zh
+00000060: 222c 2022 6b6f 225d 2c0d 0a20 2020 2020  ", "ko"],..     
+00000070: 2020 2020 2020 2022 6c61 6e67 5f63 6f64         "lang_cod
+00000080: 6522 3a20 2265 6173 796f 6372 220d 0a20  e": "easyocr".. 
+00000090: 2020 2020 2020 207d 0d0a 2020 2020 5d2c         }..    ],
+000000a0: 0d0a 2020 2020 226f 6372 223a 205b 0d0a  ..    "ocr": [..
+000000b0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+000000c0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+000000d0: 6b68 612d 7768 6974 652f 6d61 6e67 612d  kha-white/manga-
+000000e0: 6f63 722d 6261 7365 222c 0d0a 2020 2020  ocr-base",..    
+000000f0: 2020 2020 2020 2020 226c 616e 6722 3a20          "lang": 
+00000100: 5b22 6a61 225d 2c0d 0a20 2020 2020 2020  ["ja"],..       
+00000110: 2020 2020 2022 6c61 6e67 5f63 6f64 6522       "lang_code"
+00000120: 3a20 2269 736f 3122 0d0a 2020 2020 2020  : "iso1"..      
+00000130: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
+00000140: 0a20 2020 2020 2020 2020 2020 2022 6e61  .            "na
+00000150: 6d65 223a 2022 7465 7373 6572 6163 7422  me": "tesseract"
+00000160: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000170: 6c61 6e67 223a 205b 2265 6e22 2c20 226a  lang": ["en", "j
+00000180: 6122 2c20 227a 6822 2c20 226b 6f22 5d2c  a", "zh", "ko"],
+00000190: 0d0a 2020 2020 2020 2020 2020 2020 226c  ..            "l
+000001a0: 616e 675f 636f 6465 223a 2022 7465 7373  ang_code": "tess
+000001b0: 6572 6163 7422 0d0a 2020 2020 2020 2020  eract"..        
+000001c0: 7d0d 0a20 2020 205d 2c0d 0a20 2020 2022  }..    ],..    "
+000001d0: 7473 6c22 3a20 5b0d 0a20 2020 2020 2020  tsl": [..       
+000001e0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000001f0: 226e 616d 6522 3a20 2248 656c 7369 6e6b  "name": "Helsink
+00000200: 692d 4e4c 502f 6f70 7573 2d6d 742d 7a68  i-NLP/opus-mt-zh
+00000210: 2d65 6e22 2c0d 0a20 2020 2020 2020 2020  -en",..         
+00000220: 2020 2022 6c61 6e67 5f73 7263 223a 205b     "lang_src": [
+00000230: 227a 6822 5d2c 0d0a 2020 2020 2020 2020  "zh"],..        
+00000240: 2020 2020 226c 616e 675f 6473 7422 3a20      "lang_dst": 
+00000250: 5b22 656e 225d 2c0d 0a20 2020 2020 2020  ["en"],..       
+00000260: 2020 2020 2022 6c61 6e67 5f63 6f64 6522       "lang_code"
+00000270: 3a20 2269 736f 3122 0d0a 2020 2020 2020  : "iso1"..      
+00000280: 2020 7d2c 0d0a 2020 2020 2020 2020 7b0d    },..        {.
+00000290: 0a20 2020 2020 2020 2020 2020 2022 6e61  .            "na
+000002a0: 6d65 223a 2022 4865 6c73 696e 6b69 2d4e  me": "Helsinki-N
+000002b0: 4c50 2f6f 7075 732d 6d74 2d6a 612d 656e  LP/opus-mt-ja-en
+000002c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000002d0: 226c 616e 675f 7372 6322 3a20 5b22 6a61  "lang_src": ["ja
+000002e0: 225d 2c0d 0a20 2020 2020 2020 2020 2020  "],..           
+000002f0: 2022 6c61 6e67 5f64 7374 223a 205b 2265   "lang_dst": ["e
+00000300: 6e22 5d2c 0d0a 2020 2020 2020 2020 2020  n"],..          
+00000310: 2020 226c 616e 675f 636f 6465 223a 2022    "lang_code": "
+00000320: 6973 6f31 220d 0a20 2020 2020 2020 207d  iso1"..        }
+00000330: 2c0d 0a20 2020 2020 2020 207b 0d0a 2020  ,..        {..  
+00000340: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00000350: 3a20 2273 7461 6b61 2f66 7567 756d 742d  : "staka/fugumt-
+00000360: 6a61 2d65 6e22 2c0d 0a20 2020 2020 2020  ja-en",..       
+00000370: 2020 2020 2022 6c61 6e67 5f73 7263 223a       "lang_src":
+00000380: 205b 226a 6122 5d2c 0d0a 2020 2020 2020   ["ja"],..      
+00000390: 2020 2020 2020 226c 616e 675f 6473 7422        "lang_dst"
+000003a0: 3a20 5b22 656e 225d 2c0d 0a20 2020 2020  : ["en"],..     
+000003b0: 2020 2020 2020 2022 6c61 6e67 5f63 6f64         "lang_cod
+000003c0: 6522 3a20 2269 736f 3122 0d0a 2020 2020  e": "iso1"..    
+000003d0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
+000003e0: 7b0d 0a20 2020 2020 2020 2020 2020 2022  {..            "
+000003f0: 6e61 6d65 223a 2022 4865 6c73 696e 6b69  name": "Helsinki
+00000400: 2d4e 4c50 2f6f 7075 732d 6d74 2d6b 6f2d  -NLP/opus-mt-ko-
+00000410: 656e 222c 0d0a 2020 2020 2020 2020 2020  en",..          
+00000420: 2020 226c 616e 675f 7372 6322 3a20 5b22    "lang_src": ["
+00000430: 6b6f 225d 2c0d 0a20 2020 2020 2020 2020  ko"],..         
+00000440: 2020 2022 6c61 6e67 5f64 7374 223a 205b     "lang_dst": [
+00000450: 2265 6e22 5d2c 0d0a 2020 2020 2020 2020  "en"],..        
+00000460: 2020 2020 226c 616e 675f 636f 6465 223a      "lang_code":
+00000470: 2022 6973 6f31 220d 0a20 2020 2020 2020   "iso1"..       
+00000480: 207d 2c0d 0a20 2020 2020 2020 207b 0d0a   },..        {..
+00000490: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+000004a0: 6522 3a20 2266 6163 6562 6f6f 6b2f 6d32  e": "facebook/m2
+000004b0: 6d31 3030 5f34 3138 4d22 2c0d 0a20 2020  m100_418M",..   
+000004c0: 2020 2020 2020 2020 2022 6c61 6e67 5f73           "lang_s
+000004d0: 7263 223a 205b 2261 6622 2c20 2261 6d22  rc": ["af", "am"
+000004e0: 2c20 2261 7222 2c20 2261 7a22 2c20 2262  , "ar", "az", "b
+000004f0: 6122 2c20 2262 6522 2c20 2262 6722 2c20  a", "be", "bg", 
+00000500: 2262 6e22 2c20 2262 7222 2c20 2262 7322  "bn", "br", "bs"
+00000510: 2c20 2263 7322 2c20 2263 7922 2c20 2264  , "cs", "cy", "d
+00000520: 6122 2c20 2264 6522 2c20 2265 6e22 2c20  a", "de", "en", 
+00000530: 2265 7422 2c20 2266 6122 2c20 2266 6622  "et", "fa", "ff"
+00000540: 2c20 2266 6922 2c20 2266 7222 2c20 2266  , "fi", "fr", "f
+00000550: 7922 2c20 2267 6122 2c20 2267 6c22 2c20  y", "ga", "gl", 
+00000560: 2267 7522 2c20 2268 6122 2c20 2268 6522  "gu", "ha", "he"
+00000570: 2c20 2268 6922 2c20 2268 7222 2c20 2268  , "hi", "hr", "h
+00000580: 7522 2c20 2268 7922 2c20 2269 6422 2c20  u", "hy", "id", 
+00000590: 2269 6722 2c20 2269 7322 2c20 2269 7422  "ig", "is", "it"
+000005a0: 2c20 226a 6122 2c20 226a 7622 2c20 226b  , "ja", "jv", "k
+000005b0: 6122 2c20 226b 6b22 2c20 226b 6d22 2c20  a", "kk", "km", 
+000005c0: 226b 6e22 2c20 226b 6f22 2c20 226c 6722  "kn", "ko", "lg"
+000005d0: 2c20 226c 6e22 2c20 226c 6f22 2c20 226c  , "ln", "lo", "l
+000005e0: 7422 2c20 226c 7622 2c20 226d 6722 2c20  t", "lv", "mg", 
+000005f0: 226d 6b22 2c20 226d 6c22 2c20 226d 6e22  "mk", "ml", "mn"
+00000600: 2c20 226d 7222 2c20 226d 7322 2c20 226d  , "mr", "ms", "m
+00000610: 7922 2c20 226e 6522 2c20 226e 6f22 2c20  y", "ne", "no", 
+00000620: 226f 6322 2c20 226f 7222 2c20 2270 6c22  "oc", "or", "pl"
+00000630: 2c20 2270 7422 2c20 2272 7522 2c20 2273  , "pt", "ru", "s
+00000640: 6422 2c20 2273 6b22 2c20 2273 6c22 2c20  d", "sk", "sl", 
+00000650: 2273 6f22 2c20 2273 7122 2c20 2273 7222  "so", "sq", "sr"
+00000660: 2c20 2273 7322 2c20 2273 7522 2c20 2273  , "ss", "su", "s
+00000670: 7622 2c20 2273 7722 2c20 2274 6122 2c20  v", "sw", "ta", 
+00000680: 2274 6822 2c20 2274 6c22 2c20 2274 6e22  "th", "tl", "tn"
+00000690: 2c20 2274 7222 2c20 2275 6b22 2c20 2275  , "tr", "uk", "u
+000006a0: 7222 2c20 2275 7a22 2c20 2276 6922 2c20  r", "uz", "vi", 
+000006b0: 2277 6f22 2c20 2278 6822 2c20 2279 6922  "wo", "xh", "yi"
+000006c0: 2c20 2279 6f22 2c20 227a 6822 2c20 227a  , "yo", "zh", "z
+000006d0: 7522 5d2c 0d0a 2020 2020 2020 2020 2020  u"],..          
+000006e0: 2020 226c 616e 675f 6473 7422 3a20 5b22    "lang_dst": ["
+000006f0: 6166 222c 2022 616d 222c 2022 6172 222c  af", "am", "ar",
+00000700: 2022 617a 222c 2022 6261 222c 2022 6265   "az", "ba", "be
+00000710: 222c 2022 6267 222c 2022 626e 222c 2022  ", "bg", "bn", "
+00000720: 6272 222c 2022 6273 222c 2022 6373 222c  br", "bs", "cs",
+00000730: 2022 6379 222c 2022 6461 222c 2022 6465   "cy", "da", "de
+00000740: 222c 2022 656e 222c 2022 6574 222c 2022  ", "en", "et", "
+00000750: 6661 222c 2022 6666 222c 2022 6669 222c  fa", "ff", "fi",
+00000760: 2022 6672 222c 2022 6679 222c 2022 6761   "fr", "fy", "ga
+00000770: 222c 2022 676c 222c 2022 6775 222c 2022  ", "gl", "gu", "
+00000780: 6861 222c 2022 6865 222c 2022 6869 222c  ha", "he", "hi",
+00000790: 2022 6872 222c 2022 6875 222c 2022 6879   "hr", "hu", "hy
+000007a0: 222c 2022 6964 222c 2022 6967 222c 2022  ", "id", "ig", "
+000007b0: 6973 222c 2022 6974 222c 2022 6a61 222c  is", "it", "ja",
+000007c0: 2022 6a76 222c 2022 6b61 222c 2022 6b6b   "jv", "ka", "kk
+000007d0: 222c 2022 6b6d 222c 2022 6b6e 222c 2022  ", "km", "kn", "
+000007e0: 6b6f 222c 2022 6c67 222c 2022 6c6e 222c  ko", "lg", "ln",
+000007f0: 2022 6c6f 222c 2022 6c74 222c 2022 6c76   "lo", "lt", "lv
+00000800: 222c 2022 6d67 222c 2022 6d6b 222c 2022  ", "mg", "mk", "
+00000810: 6d6c 222c 2022 6d6e 222c 2022 6d72 222c  ml", "mn", "mr",
+00000820: 2022 6d73 222c 2022 6d79 222c 2022 6e65   "ms", "my", "ne
+00000830: 222c 2022 6e6f 222c 2022 6f63 222c 2022  ", "no", "oc", "
+00000840: 6f72 222c 2022 706c 222c 2022 7074 222c  or", "pl", "pt",
+00000850: 2022 7275 222c 2022 7364 222c 2022 736b   "ru", "sd", "sk
+00000860: 222c 2022 736c 222c 2022 736f 222c 2022  ", "sl", "so", "
+00000870: 7371 222c 2022 7372 222c 2022 7373 222c  sq", "sr", "ss",
+00000880: 2022 7375 222c 2022 7376 222c 2022 7377   "su", "sv", "sw
+00000890: 222c 2022 7461 222c 2022 7468 222c 2022  ", "ta", "th", "
+000008a0: 746c 222c 2022 746e 222c 2022 7472 222c  tl", "tn", "tr",
+000008b0: 2022 756b 222c 2022 7572 222c 2022 757a   "uk", "ur", "uz
+000008c0: 222c 2022 7669 222c 2022 776f 222c 2022  ", "vi", "wo", "
+000008d0: 7868 222c 2022 7969 222c 2022 796f 222c  xh", "yi", "yo",
+000008e0: 2022 7a68 222c 2022 7a75 225d 2c0d 0a20   "zh", "zu"],.. 
+000008f0: 2020 2020 2020 2020 2020 2022 6c61 6e67             "lang
+00000900: 5f63 6f64 6522 3a20 2266 6163 6562 6f6f  _code": "faceboo
+00000910: 6b4d 324d 220d 0a20 2020 2020 2020 207d  kM2M"..        }
+00000920: 2c0d 0a20 2020 2020 2020 207b 0d0a 2020  ,..        {..  
+00000930: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00000940: 3a20 2266 6163 6562 6f6f 6b2f 6d32 6d31  : "facebook/m2m1
+00000950: 3030 5f31 2e32 4222 2c0d 0a20 2020 2020  00_1.2B",..     
+00000960: 2020 2020 2020 2022 6c61 6e67 5f73 7263         "lang_src
+00000970: 223a 205b 2261 6622 2c20 2261 6d22 2c20  ": ["af", "am", 
+00000980: 2261 7222 2c20 2261 7a22 2c20 2262 6122  "ar", "az", "ba"
+00000990: 2c20 2262 6522 2c20 2262 6722 2c20 2262  , "be", "bg", "b
+000009a0: 6e22 2c20 2262 7222 2c20 2262 7322 2c20  n", "br", "bs", 
+000009b0: 2263 7322 2c20 2263 7922 2c20 2264 6122  "cs", "cy", "da"
+000009c0: 2c20 2264 6522 2c20 2265 6e22 2c20 2265  , "de", "en", "e
+000009d0: 7422 2c20 2266 6122 2c20 2266 6622 2c20  t", "fa", "ff", 
+000009e0: 2266 6922 2c20 2266 7222 2c20 2266 7922  "fi", "fr", "fy"
+000009f0: 2c20 2267 6122 2c20 2267 6c22 2c20 2267  , "ga", "gl", "g
+00000a00: 7522 2c20 2268 6122 2c20 2268 6522 2c20  u", "ha", "he", 
+00000a10: 2268 6922 2c20 2268 7222 2c20 2268 7522  "hi", "hr", "hu"
+00000a20: 2c20 2268 7922 2c20 2269 6422 2c20 2269  , "hy", "id", "i
+00000a30: 6722 2c20 2269 7322 2c20 2269 7422 2c20  g", "is", "it", 
+00000a40: 226a 6122 2c20 226a 7622 2c20 226b 6122  "ja", "jv", "ka"
+00000a50: 2c20 226b 6b22 2c20 226b 6d22 2c20 226b  , "kk", "km", "k
+00000a60: 6e22 2c20 226b 6f22 2c20 226c 6722 2c20  n", "ko", "lg", 
+00000a70: 226c 6e22 2c20 226c 6f22 2c20 226c 7422  "ln", "lo", "lt"
+00000a80: 2c20 226c 7622 2c20 226d 6722 2c20 226d  , "lv", "mg", "m
+00000a90: 6b22 2c20 226d 6c22 2c20 226d 6e22 2c20  k", "ml", "mn", 
+00000aa0: 226d 7222 2c20 226d 7322 2c20 226d 7922  "mr", "ms", "my"
+00000ab0: 2c20 226e 6522 2c20 226e 6f22 2c20 226f  , "ne", "no", "o
+00000ac0: 6322 2c20 226f 7222 2c20 2270 6c22 2c20  c", "or", "pl", 
+00000ad0: 2270 7422 2c20 2272 7522 2c20 2273 6422  "pt", "ru", "sd"
+00000ae0: 2c20 2273 6b22 2c20 2273 6c22 2c20 2273  , "sk", "sl", "s
+00000af0: 6f22 2c20 2273 7122 2c20 2273 7222 2c20  o", "sq", "sr", 
+00000b00: 2273 7322 2c20 2273 7522 2c20 2273 7622  "ss", "su", "sv"
+00000b10: 2c20 2273 7722 2c20 2274 6122 2c20 2274  , "sw", "ta", "t
+00000b20: 6822 2c20 2274 6c22 2c20 2274 6e22 2c20  h", "tl", "tn", 
+00000b30: 2274 7222 2c20 2275 6b22 2c20 2275 7222  "tr", "uk", "ur"
+00000b40: 2c20 2275 7a22 2c20 2276 6922 2c20 2277  , "uz", "vi", "w
+00000b50: 6f22 2c20 2278 6822 2c20 2279 6922 2c20  o", "xh", "yi", 
+00000b60: 2279 6f22 2c20 227a 6822 2c20 227a 7522  "yo", "zh", "zu"
+00000b70: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00000b80: 226c 616e 675f 6473 7422 3a20 5b22 6166  "lang_dst": ["af
+00000b90: 222c 2022 616d 222c 2022 6172 222c 2022  ", "am", "ar", "
+00000ba0: 617a 222c 2022 6261 222c 2022 6265 222c  az", "ba", "be",
+00000bb0: 2022 6267 222c 2022 626e 222c 2022 6272   "bg", "bn", "br
+00000bc0: 222c 2022 6273 222c 2022 6373 222c 2022  ", "bs", "cs", "
+00000bd0: 6379 222c 2022 6461 222c 2022 6465 222c  cy", "da", "de",
+00000be0: 2022 656e 222c 2022 6574 222c 2022 6661   "en", "et", "fa
+00000bf0: 222c 2022 6666 222c 2022 6669 222c 2022  ", "ff", "fi", "
+00000c00: 6672 222c 2022 6679 222c 2022 6761 222c  fr", "fy", "ga",
+00000c10: 2022 676c 222c 2022 6775 222c 2022 6861   "gl", "gu", "ha
+00000c20: 222c 2022 6865 222c 2022 6869 222c 2022  ", "he", "hi", "
+00000c30: 6872 222c 2022 6875 222c 2022 6879 222c  hr", "hu", "hy",
+00000c40: 2022 6964 222c 2022 6967 222c 2022 6973   "id", "ig", "is
+00000c50: 222c 2022 6974 222c 2022 6a61 222c 2022  ", "it", "ja", "
+00000c60: 6a76 222c 2022 6b61 222c 2022 6b6b 222c  jv", "ka", "kk",
+00000c70: 2022 6b6d 222c 2022 6b6e 222c 2022 6b6f   "km", "kn", "ko
+00000c80: 222c 2022 6c67 222c 2022 6c6e 222c 2022  ", "lg", "ln", "
+00000c90: 6c6f 222c 2022 6c74 222c 2022 6c76 222c  lo", "lt", "lv",
+00000ca0: 2022 6d67 222c 2022 6d6b 222c 2022 6d6c   "mg", "mk", "ml
+00000cb0: 222c 2022 6d6e 222c 2022 6d72 222c 2022  ", "mn", "mr", "
+00000cc0: 6d73 222c 2022 6d79 222c 2022 6e65 222c  ms", "my", "ne",
+00000cd0: 2022 6e6f 222c 2022 6f63 222c 2022 6f72   "no", "oc", "or
+00000ce0: 222c 2022 706c 222c 2022 7074 222c 2022  ", "pl", "pt", "
+00000cf0: 7275 222c 2022 7364 222c 2022 736b 222c  ru", "sd", "sk",
+00000d00: 2022 736c 222c 2022 736f 222c 2022 7371   "sl", "so", "sq
+00000d10: 222c 2022 7372 222c 2022 7373 222c 2022  ", "sr", "ss", "
+00000d20: 7375 222c 2022 7376 222c 2022 7377 222c  su", "sv", "sw",
+00000d30: 2022 7461 222c 2022 7468 222c 2022 746c   "ta", "th", "tl
+00000d40: 222c 2022 746e 222c 2022 7472 222c 2022  ", "tn", "tr", "
+00000d50: 756b 222c 2022 7572 222c 2022 757a 222c  uk", "ur", "uz",
+00000d60: 2022 7669 222c 2022 776f 222c 2022 7868   "vi", "wo", "xh
+00000d70: 222c 2022 7969 222c 2022 796f 222c 2022  ", "yi", "yo", "
+00000d80: 7a68 222c 2022 7a75 225d 2c0d 0a20 2020  zh", "zu"],..   
+00000d90: 2020 2020 2020 2020 2022 6c61 6e67 5f63           "lang_c
+00000da0: 6f64 6522 3a20 2266 6163 6562 6f6f 6b4d  ode": "facebookM
+00000db0: 324d 220d 0a20 2020 2020 2020 207d 0d0a  2M"..        }..
+00000dc0: 2020 2020 5d0d 0a7d                          ]..}
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/OCR_TSL/tesseract.py` & `django_ocr_translate-0.1.3/ocr_translate/ocr_tsl/tesseract.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,132 @@
-###################################################################################
-# ocr_translate - a django app to perform OCR and translation of images.          #
-# Copyright (C) 2023-present Davide Grassano                                      #
-#                                                                                 #
-# This program is free software: you can redistribute it and/or modify            #
-# it under the terms of the GNU General Public License as published by            #
-# the Free Software Foundation, either version 3 of the License.                  #
-#                                                                                 #
-# This program is distributed in the hope that it will be useful,                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
-# GNU General Public License for more details.                                    #
-#                                                                                 #
-# You should have received a copy of the GNU General Public License               #
-# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
-#                                                                                 #
-# Home: https://github.com/Crivella/ocr_translate                                 #
-###################################################################################
-import logging
-import os
-from pathlib import Path
-
-import requests
-from PIL import Image
-from pytesseract import Output, image_to_string
-
-from .base import root
-
-logger = logging.getLogger('ocr.general')
-
-model_url = 'https://github.com/tesseract-ocr/tessdata_best/raw/main/{}.traineddata'
-
-data_dir = Path(os.getenv('TESSERACT_PREFIX', root / 'tesseract'))
-
-vertical_langs = ['jpn', 'chi_tra', 'chi_sim', 'kor']
-
-download = os.getenv('TESSERACT_ALLOW_DOWNLOAD', 'false').lower() == 'true'
-config = False
-
-def download_model(lang: str):
-    if not download:
-        raise ValueError('Downloading models is not allowed')
-    create_config()
-    
-    logger.info(f'Downloading tesseract model for language {lang}')
-    dst = data_dir / f'{lang}.traineddata'
-    if dst.exists():
-        return
-    res = requests.get(model_url.format(lang))
-    if res.status_code != 200:
-        raise ValueError(f'Could not download model for language {lang}')
-    
-    with open(data_dir / f'{lang}.traineddata', 'wb') as f:
-        f.write(res.content)
-
-    if lang in vertical_langs:
-        download_model(lang + '_vert')
-
-def create_config():
-    global config
-    if config:
-        return
-    config = True
-    
-    logger.info('Creating tesseract tsv config')
-    cfg = data_dir / 'configs'
-    cfg.mkdir(exist_ok=True, parents=True)
-
-    dst = cfg / 'tsv'
-    if dst.exists():
-        return
-    with dst.open('w') as f:
-        f.write('tessedit_create_tsv 1')
-
-# Page segmentation modes:
-#   0    Orientation and script detection (OSD) only.
-#   1    Automatic page segmentation with OSD.
-#   2    Automatic page segmentation, but no OSD, or OCR.
-#   3    Fully automatic page segmentation, but no OSD. (Default)
-#   4    Assume a single column of text of variable sizes.
-#   5    Assume a single uniform block of vertically aligned text.
-#   6    Assume a single uniform block of text.
-#   7    Treat the image as a single text line.
-#   8    Treat the image as a single word.
-#   9    Treat the image as a single word in a circle.
-#  10    Treat the image as a single character.
-#  11    Sparse text. Find as much text as possible in no particular order.
-#  12    Sparse text with OSD.
-#  13    Raw line. Treat the image as a single text line,
-#        bypassing hacks that are Tesseract-specific.
-def tesseract_pipeline(img: Image.Image, lang: str, conf_thr: int = 15, favor_vertical: bool = True) -> str:
-    create_config()
-    if not (data_dir / f'{lang}.traineddata').exists():
-        download_model(lang)
-    logger.info(f'Running tesseract for language {lang}')
-
-    psm = 6
-    if lang in vertical_langs:
-        e = 1 if favor_vertical else -1
-        if img.height * 1.5**e > img.width:
-            psm = 5
-
-    # Using image_to_string will atleast preserve spaces
-    res = image_to_string(
-        img, 
-        lang=lang, 
-        config=f'--tessdata-dir {data_dir.as_posix()} --psm {psm}', 
-        output_type=Output.DICT
-        )
-    
-    return res['text']
+###################################################################################
+# ocr_translate - a django app to perform OCR and translation of images.          #
+# Copyright (C) 2023-present Davide Grassano                                      #
+#                                                                                 #
+# This program is free software: you can redistribute it and/or modify            #
+# it under the terms of the GNU General Public License as published by            #
+# the Free Software Foundation, either version 3 of the License.                  #
+#                                                                                 #
+# This program is distributed in the hope that it will be useful,                 #
+# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
+# GNU General Public License for more details.                                    #
+#                                                                                 #
+# You should have received a copy of the GNU General Public License               #
+# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
+#                                                                                 #
+# Home: https://github.com/Crivella/ocr_translate                                 #
+###################################################################################
+"""Functions and piplines to perform OCR on images using tesseract."""
+import logging
+import os
+from pathlib import Path
+
+import requests
+from PIL import Image
+from pytesseract import Output, image_to_string
+
+from .huggingface import root
+
+logger = logging.getLogger('ocr.general')
+
+MODEL_URL = 'https://github.com/tesseract-ocr/tessdata_best/raw/main/{}.traineddata'
+
+DATA_DIR = Path(os.getenv('TESSERACT_PREFIX', root / 'tesseract'))
+
+VERTICAL_LANGS = ['jpn', 'chi_tra', 'chi_sim', 'kor']
+
+DOWNLOAD = os.getenv('TESSERACT_ALLOW_DOWNLOAD', 'false').lower() == 'true'
+CONFIG = False
+
+def download_model(lang: str):
+    """Download a tesseract model for a given language.
+
+    Args:
+        lang (str): A language code for tesseract.
+
+    Raises:
+        ValueError: If the model could not be downloaded.
+    """
+    if not DOWNLOAD:
+        raise ValueError('TESSERACT_ALLOW_DOWNLOAD is false. Downloading models is not allowed')
+    create_config()
+
+    logger.info(f'Downloading tesseract model for language {lang}')
+    dst = DATA_DIR / f'{lang}.traineddata'
+    if dst.exists():
+        return
+    res = requests.get(MODEL_URL.format(lang), timeout=5)
+    if res.status_code != 200:
+        raise ValueError(f'Could not download model for language {lang}')
+
+    with open(DATA_DIR / f'{lang}.traineddata', 'wb') as f:
+        f.write(res.content)
+
+    if lang in VERTICAL_LANGS:
+        download_model(lang + '_vert')
+
+def create_config():
+    """Create a tesseract config file. Run only once"""
+    global CONFIG
+    if CONFIG:
+        return
+    CONFIG = True
+
+    logger.info('Creating tesseract tsv config')
+    cfg = DATA_DIR / 'configs'
+    cfg.mkdir(exist_ok=True, parents=True)
+
+    dst = cfg / 'tsv'
+    if dst.exists():
+        return
+    with dst.open('w') as f:
+        f.write('tessedit_create_tsv 1')
+
+# Page segmentation modes:
+#   0    Orientation and script detection (OSD) only.
+#   1    Automatic page segmentation with OSD.
+#   2    Automatic page segmentation, but no OSD, or OCR.
+#   3    Fully automatic page segmentation, but no OSD. (Default)
+#   4    Assume a single column of text of variable sizes.
+#   5    Assume a single uniform block of vertically aligned text.
+#   6    Assume a single uniform block of text.
+#   7    Treat the image as a single text line.
+#   8    Treat the image as a single word.
+#   9    Treat the image as a single word in a circle.
+#  10    Treat the image as a single character.
+#  11    Sparse text. Find as much text as possible in no particular order.
+#  12    Sparse text with OSD.
+#  13    Raw line. Treat the image as a single text line,
+#        bypassing hacks that are Tesseract-specific.
+def tesseract_pipeline(img: Image.Image, lang: str, favor_vertical: bool = True) -> str:
+    """Run tesseract on an image.
+
+    Args:
+        img (Image.Image): An image to run tesseract on.
+        lang (str): A language code for tesseract.
+        favor_vertical (bool, optional): Wether to favor vertical or horizontal configuration for languages that
+            can be written vertically. Defaults to True.
+
+    Returns:
+        str: The text extracted from the image.
+    """    """"""
+    create_config()
+    if not (DATA_DIR / f'{lang}.traineddata').exists():
+        download_model(lang)
+    logger.info(f'Running tesseract for language {lang}')
+
+    psm = 6
+    if lang in VERTICAL_LANGS:
+        exp = 1 if favor_vertical else -1
+        if img.height * 1.5**exp > img.width:
+            psm = 5
+
+    # Using image_to_string will atleast preserve spaces
+    res = image_to_string(
+        img,
+        lang=lang,
+        config=f'--tessdata-dir {DATA_DIR.as_posix()} --psm {psm}',
+        output_type=Output.DICT
+        )
+
+    return res['text']
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/__init__.py` & `django_ocr_translate-0.1.3/ocr_translate/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-###################################################################################
-# ocr_translate - a django app to perform OCR and translation of images.          #
-# Copyright (C) 2023-present Davide Grassano                                      #
-#                                                                                 #
-# This program is free software: you can redistribute it and/or modify            #
-# it under the terms of the GNU General Public License as published by            #
-# the Free Software Foundation, either version 3 of the License.                  #
-#                                                                                 #
-# This program is distributed in the hope that it will be useful,                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
-# GNU General Public License for more details.                                    #
-#                                                                                 #
-# You should have received a copy of the GNU General Public License               #
-# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
-#                                                                                 #
-# Home: https://github.com/Crivella/ocr_translate                                 #
-###################################################################################
-
-
-__version__ = '0.1.2'
+###################################################################################
+# ocr_translate - a django app to perform OCR and translation of images.          #
+# Copyright (C) 2023-present Davide Grassano                                      #
+#                                                                                 #
+# This program is free software: you can redistribute it and/or modify            #
+# it under the terms of the GNU General Public License as published by            #
+# the Free Software Foundation, either version 3 of the License.                  #
+#                                                                                 #
+# This program is distributed in the hope that it will be useful,                 #
+# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
+# GNU General Public License for more details.                                    #
+#                                                                                 #
+# You should have received a copy of the GNU General Public License               #
+# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
+#                                                                                 #
+# Home: https://github.com/Crivella/ocr_translate                                 #
+###################################################################################
+"""OCR and translation of images."""
+
+__version__ = '0.1.3'
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/admin.py` & `django_ocr_translate-0.1.3/ocr_translate/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-###################################################################################
-# ocr_translate - a django app to perform OCR and translation of images.          #
-# Copyright (C) 2023-present Davide Grassano                                      #
-#                                                                                 #
-# This program is free software: you can redistribute it and/or modify            #
-# it under the terms of the GNU General Public License as published by            #
-# the Free Software Foundation, either version 3 of the License.                  #
-#                                                                                 #
-# This program is distributed in the hope that it will be useful,                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
-# GNU General Public License for more details.                                    #
-#                                                                                 #
-# You should have received a copy of the GNU General Public License               #
-# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
-#                                                                                 #
-# Home: https://github.com/Crivella/ocr_translate                                 #
-###################################################################################
-from django.contrib import admin
-
-from . import models as m
-
-# Register your models here.
-
-class LanguageAdmin(admin.ModelAdmin):
-    list_display = ('name', 'iso1', 'iso2b', 'iso2t', 'iso3')
-
-class OCRBoxModelAdmin(admin.ModelAdmin):
-    list_display = ('name',)
-
-class OCRModelAdmin(admin.ModelAdmin):
-    list_display = ('name',)
-
-class TSLModelAdmin(admin.ModelAdmin):
-    list_display = ('name',)
-
-
-admin.site.register(m.Language, LanguageAdmin)
-admin.site.register(m.OCRBoxModel, OCRBoxModelAdmin)
-admin.site.register(m.OCRModel, OCRModelAdmin)
-admin.site.register(m.TSLModel, TSLModelAdmin)
+###################################################################################
+# ocr_translate - a django app to perform OCR and translation of images.          #
+# Copyright (C) 2023-present Davide Grassano                                      #
+#                                                                                 #
+# This program is free software: you can redistribute it and/or modify            #
+# it under the terms of the GNU General Public License as published by            #
+# the Free Software Foundation, either version 3 of the License.                  #
+#                                                                                 #
+# This program is distributed in the hope that it will be useful,                 #
+# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
+# GNU General Public License for more details.                                    #
+#                                                                                 #
+# You should have received a copy of the GNU General Public License               #
+# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
+#                                                                                 #
+# Home: https://github.com/Crivella/ocr_translate                                 #
+###################################################################################
+"""Admin interface for ocr_translate app."""
+from django.contrib import admin
+
+from . import models as m
+
+
+class LanguageAdmin(admin.ModelAdmin):
+    """Admin interface for Language model"""
+    list_display = ('name', 'iso1', 'iso2b', 'iso2t', 'iso3')
+
+class OCRBoxModelAdmin(admin.ModelAdmin):
+    """Admin interface for OCRBoxModel model"""
+    list_display = ('name',)
+
+class OCRModelAdmin(admin.ModelAdmin):
+    """Admin interface for OCRModel model"""
+    list_display = ('name',)
+
+class TSLModelAdmin(admin.ModelAdmin):
+    """Admin interface for TSLModel model"""
+    list_display = ('name',)
+
+
+admin.site.register(m.Language, LanguageAdmin)
+admin.site.register(m.OCRBoxModel, OCRBoxModelAdmin)
+admin.site.register(m.OCRModel, OCRModelAdmin)
+admin.site.register(m.TSLModel, TSLModelAdmin)
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/apps.py` & `django_ocr_translate-0.1.3/ocr_translate/apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-###################################################################################
-# ocr_translate - a django app to perform OCR and translation of images.          #
-# Copyright (C) 2023-present Davide Grassano                                      #
-#                                                                                 #
-# This program is free software: you can redistribute it and/or modify            #
-# it under the terms of the GNU General Public License as published by            #
-# the Free Software Foundation, either version 3 of the License.                  #
-#                                                                                 #
-# This program is distributed in the hope that it will be useful,                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
-# GNU General Public License for more details.                                    #
-#                                                                                 #
-# You should have received a copy of the GNU General Public License               #
-# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
-#                                                                                 #
-# Home: https://github.com/Crivella/ocr_translate                                 #
-###################################################################################
-from django.apps import AppConfig
-
-
-class OCR_TSLconfig(AppConfig):
-    default_auto_field = 'django.db.models.BigAutoField'
-    name = 'ocr_translate'
+###################################################################################
+# ocr_translate - a django app to perform OCR and translation of images.          #
+# Copyright (C) 2023-present Davide Grassano                                      #
+#                                                                                 #
+# This program is free software: you can redistribute it and/or modify            #
+# it under the terms of the GNU General Public License as published by            #
+# the Free Software Foundation, either version 3 of the License.                  #
+#                                                                                 #
+# This program is distributed in the hope that it will be useful,                 #
+# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
+# GNU General Public License for more details.                                    #
+#                                                                                 #
+# You should have received a copy of the GNU General Public License               #
+# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
+#                                                                                 #
+# Home: https://github.com/Crivella/ocr_translate                                 #
+###################################################################################
+"""App configuration for ocr_translate."""
+from django.apps import AppConfig
+
+
+class OCRTSLconfig(AppConfig):
+    """App configuration for ocr_translate."""
+    default_auto_field = 'django.db.models.BigAutoField'
+    name = 'ocr_translate'
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/migrations/0001_initial.py` & `django_ocr_translate-0.1.3/ocr_translate/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-# Generated by Django 4.2.2 on 2023-07-17 14:12
-
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='BBox',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('l', models.IntegerField()),
-                ('b', models.IntegerField()),
-                ('r', models.IntegerField()),
-                ('t', models.IntegerField()),
-            ],
-        ),
-        migrations.CreateModel(
-            name='Image',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('md5', models.CharField(max_length=32, unique=True)),
-            ],
-        ),
-        migrations.CreateModel(
-            name='Language',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=64, unique=True)),
-                ('iso1', models.CharField(max_length=8, unique=True)),
-                ('iso2b', models.CharField(max_length=8, unique=True)),
-                ('iso2t', models.CharField(max_length=8, unique=True)),
-                ('iso3', models.CharField(max_length=32, unique=True)),
-                ('easyocr', models.CharField(max_length=32, null=True)),
-                ('tesseract', models.CharField(max_length=32, null=True)),
-                ('facebookM2M', models.CharField(max_length=32, null=True)),
-                ('break_chars', models.CharField(max_length=512, null=True)),
-                ('ignore_chars', models.CharField(max_length=512, null=True)),
-            ],
-        ),
-        migrations.CreateModel(
-            name='OCRBoxModel',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=128)),
-                ('language_format', models.CharField(max_length=32, null=True)),
-                ('languages', models.ManyToManyField(related_name='box_models', to='ocr_translate.language')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='OCRModel',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=128)),
-                ('language_format', models.CharField(max_length=32, null=True)),
-                ('languages', models.ManyToManyField(related_name='ocr_models', to='ocr_translate.language')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='OptionDict',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('options', models.JSONField(unique=True)),
-            ],
-        ),
-        migrations.CreateModel(
-            name='Text',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('text', models.TextField()),
-            ],
-        ),
-        migrations.CreateModel(
-            name='TSLModel',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=128)),
-                ('language_format', models.CharField(max_length=32, null=True)),
-                ('dst_languages', models.ManyToManyField(related_name='tsl_models_dst', to='ocr_translate.language')),
-                ('src_languages', models.ManyToManyField(related_name='tsl_models_src', to='ocr_translate.language')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='TranslationRun',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('lang_dst', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='trans_dst', to='ocr_translate.language')),
-                ('lang_src', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='trans_src', to='ocr_translate.language')),
-                ('model', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='tsl_runs', to='ocr_translate.tslmodel')),
-                ('options', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='trans_options', to='ocr_translate.optiondict')),
-                ('result', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='from_trans', to='ocr_translate.text')),
-                ('text', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='to_trans', to='ocr_translate.text')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='OCRRun',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('bbox', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='to_ocr', to='ocr_translate.bbox')),
-                ('lang_src', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ocr_src', to='ocr_translate.language')),
-                ('model', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ocr_runs', to='ocr_translate.ocrmodel')),
-                ('options', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ocr_options', to='ocr_translate.optiondict')),
-                ('result', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='from_ocr', to='ocr_translate.text')),
-            ],
-        ),
-        migrations.CreateModel(
-            name='OCRBoxRun',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('image', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='to_box', to='ocr_translate.image')),
-                ('lang_src', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='box_src', to='ocr_translate.language')),
-                ('model', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='box_runs', to='ocr_translate.ocrboxmodel')),
-                ('options', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ocr_box_options', to='ocr_translate.optiondict')),
-            ],
-        ),
-        migrations.AddField(
-            model_name='bbox',
-            name='from_ocr',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='result', to='ocr_translate.ocrboxrun'),
-        ),
-        migrations.AddField(
-            model_name='bbox',
-            name='image',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='bboxes', to='ocr_translate.image'),
-        ),
-    ]
+# Generated by Django 4.2.2 on 2023-07-17 14:12
+
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='BBox',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('l', models.IntegerField()),
+                ('b', models.IntegerField()),
+                ('r', models.IntegerField()),
+                ('t', models.IntegerField()),
+            ],
+        ),
+        migrations.CreateModel(
+            name='Image',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('md5', models.CharField(max_length=32, unique=True)),
+            ],
+        ),
+        migrations.CreateModel(
+            name='Language',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=64, unique=True)),
+                ('iso1', models.CharField(max_length=8, unique=True)),
+                ('iso2b', models.CharField(max_length=8, unique=True)),
+                ('iso2t', models.CharField(max_length=8, unique=True)),
+                ('iso3', models.CharField(max_length=32, unique=True)),
+                ('easyocr', models.CharField(max_length=32, null=True)),
+                ('tesseract', models.CharField(max_length=32, null=True)),
+                ('facebookM2M', models.CharField(max_length=32, null=True)),
+                ('break_chars', models.CharField(max_length=512, null=True)),
+                ('ignore_chars', models.CharField(max_length=512, null=True)),
+            ],
+        ),
+        migrations.CreateModel(
+            name='OCRBoxModel',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=128)),
+                ('language_format', models.CharField(max_length=32, null=True)),
+                ('languages', models.ManyToManyField(related_name='box_models', to='ocr_translate.language')),
+            ],
+        ),
+        migrations.CreateModel(
+            name='OCRModel',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=128)),
+                ('language_format', models.CharField(max_length=32, null=True)),
+                ('languages', models.ManyToManyField(related_name='ocr_models', to='ocr_translate.language')),
+            ],
+        ),
+        migrations.CreateModel(
+            name='OptionDict',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('options', models.JSONField(unique=True)),
+            ],
+        ),
+        migrations.CreateModel(
+            name='Text',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('text', models.TextField()),
+            ],
+        ),
+        migrations.CreateModel(
+            name='TSLModel',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=128)),
+                ('language_format', models.CharField(max_length=32, null=True)),
+                ('dst_languages', models.ManyToManyField(related_name='tsl_models_dst', to='ocr_translate.language')),
+                ('src_languages', models.ManyToManyField(related_name='tsl_models_src', to='ocr_translate.language')),
+            ],
+        ),
+        migrations.CreateModel(
+            name='TranslationRun',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('lang_dst', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='trans_dst', to='ocr_translate.language')),
+                ('lang_src', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='trans_src', to='ocr_translate.language')),
+                ('model', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='tsl_runs', to='ocr_translate.tslmodel')),
+                ('options', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='trans_options', to='ocr_translate.optiondict')),
+                ('result', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='from_trans', to='ocr_translate.text')),
+                ('text', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='to_trans', to='ocr_translate.text')),
+            ],
+        ),
+        migrations.CreateModel(
+            name='OCRRun',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('bbox', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='to_ocr', to='ocr_translate.bbox')),
+                ('lang_src', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ocr_src', to='ocr_translate.language')),
+                ('model', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ocr_runs', to='ocr_translate.ocrmodel')),
+                ('options', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ocr_options', to='ocr_translate.optiondict')),
+                ('result', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='from_ocr', to='ocr_translate.text')),
+            ],
+        ),
+        migrations.CreateModel(
+            name='OCRBoxRun',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('image', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='to_box', to='ocr_translate.image')),
+                ('lang_src', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='box_src', to='ocr_translate.language')),
+                ('model', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='box_runs', to='ocr_translate.ocrboxmodel')),
+                ('options', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='ocr_box_options', to='ocr_translate.optiondict')),
+            ],
+        ),
+        migrations.AddField(
+            model_name='bbox',
+            name='from_ocr',
+            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='result', to='ocr_translate.ocrboxrun'),
+        ),
+        migrations.AddField(
+            model_name='bbox',
+            name='image',
+            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='bboxes', to='ocr_translate.image'),
+        ),
+    ]
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/models.py` & `django_ocr_translate-0.1.3/ocr_translate/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-###################################################################################
-# ocr_translate - a django app to perform OCR and translation of images.          #
-# Copyright (C) 2023-present Davide Grassano                                      #
-#                                                                                 #
-# This program is free software: you can redistribute it and/or modify            #
-# it under the terms of the GNU General Public License as published by            #
-# the Free Software Foundation, either version 3 of the License.                  #
-#                                                                                 #
-# This program is distributed in the hope that it will be useful,                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
-# GNU General Public License for more details.                                    #
-#                                                                                 #
-# You should have received a copy of the GNU General Public License               #
-# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
-#                                                                                 #
-# Home: https://github.com/Crivella/ocr_translate                                 #
-###################################################################################
-from django.db import models
-
-lang_length = 32
-
-class OptionDict(models.Model):
-    """Dictionary of options for OCR and translation"""
-    options = models.JSONField(unique=True)
-
-    def __str__(self):
-        return str(self.options)
-
-class Language(models.Model):
-    """Language used for translation"""
-    name = models.CharField(max_length=64, unique=True)
-    iso1 = models.CharField(max_length=8, unique=True)
-    iso2b = models.CharField(max_length=8, unique=True)
-    iso2t = models.CharField(max_length=8, unique=True)
-    iso3 = models.CharField(max_length=32, unique=True)
-
-    easyocr = models.CharField(max_length=32, null=True)
-    tesseract = models.CharField(max_length=32, null=True)
-    facebookM2M = models.CharField(max_length=32, null=True)
-
-    break_chars = models.CharField(max_length=512, null=True)
-    ignore_chars = models.CharField(max_length=512, null=True) 
-
-    def __str__(self):
-        return str(self.iso1)
-
-class OCRModel(models.Model):
-    """OCR model using hugging space naming convention"""
-    name = models.CharField(max_length=128)
-    languages = models.ManyToManyField(Language, related_name='ocr_models')
-
-    language_format = models.CharField(max_length=32, null=True)
-
-    def __str__(self):
-        return str(self.name)
-
-class OCRBoxModel(models.Model):
-    """OCR model for bounding boxes"""
-    name = models.CharField(max_length=128)
-    languages = models.ManyToManyField(Language, related_name='box_models')
-
-    language_format = models.CharField(max_length=32, null=True)
-
-    def __str__(self):
-        return str(self.name)
-
-class TSLModel(models.Model):
-    """Translation models using hugging space naming convention"""
-    name = models.CharField(max_length=128)
-    src_languages = models.ManyToManyField(Language, related_name='tsl_models_src')
-    dst_languages = models.ManyToManyField(Language, related_name='tsl_models_dst')
-
-    language_format = models.CharField(max_length=32, null=True)
-    
-    def __str__(self):
-        return str(self.name)
-
-class Image(models.Model):
-    """Image registered as the md5 of the uploaded file"""
-    md5 = models.CharField(max_length=32, unique=True)
-
-class BBox(models.Model):
-    """Bounding box of a text in an image"""
-    l = models.IntegerField(null=False)
-    b = models.IntegerField(null=False)
-    r = models.IntegerField(null=False)
-    t = models.IntegerField(null=False)
-
-    image = models.ForeignKey(Image, on_delete=models.CASCADE, related_name='bboxes')
-    from_ocr = models.ForeignKey('OCRBoxRun', on_delete=models.CASCADE, related_name='result')
-
-    @property
-    def lbrt(self):
-        return self.l, self.b, self.r, self.t
-    
-    def __str__(self):
-        return f'{self.lbrt}'
-    
-class Text(models.Model):
-    """Text extracted from an image or translated from another text"""
-    text = models.TextField()
-    # lang = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='texts')
-
-class OCRBoxRun(models.Model):
-    """OCR run on an image using a specific model"""
-    options = models.ForeignKey(OptionDict, on_delete=models.CASCADE, related_name='ocr_box_options')
-
-    lang_src = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='box_src')
-
-    image = models.ForeignKey(Image, on_delete=models.CASCADE, related_name='to_box')
-    model = models.ForeignKey(OCRBoxModel, on_delete=models.CASCADE, related_name='box_runs')
-    # result = models.ForeignKey(BBox, on_delete=models.CASCADE, related_name='from_ocr')
-
-class OCRRun(models.Model):
-    """OCR run on an image using a specific model"""
-    options = models.ForeignKey(OptionDict, on_delete=models.CASCADE, related_name='ocr_options')
-
-    lang_src = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='ocr_src')
-
-    # image = models.ForeignKey(Image, on_delete=models.CASCADE, related_name='to_ocr')
-    bbox = models.ForeignKey(BBox, on_delete=models.CASCADE, related_name='to_ocr')
-    model = models.ForeignKey(OCRModel, on_delete=models.CASCADE, related_name='ocr_runs')
-    result = models.ForeignKey(Text, on_delete=models.CASCADE, related_name='from_ocr')
-    
-class TranslationRun(models.Model):
-    """Translation run on a text using a specific model"""
-    options = models.ForeignKey(OptionDict, on_delete=models.CASCADE, related_name='trans_options')
-
-    lang_src = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='trans_src')
-    lang_dst = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='trans_dst')
-    
-    text = models.ForeignKey(Text, on_delete=models.CASCADE, related_name='to_trans')
-    model = models.ForeignKey(TSLModel, on_delete=models.CASCADE, related_name='tsl_runs')
-    result = models.ForeignKey(Text, on_delete=models.CASCADE, related_name='from_trans')
-    
-
+###################################################################################
+# ocr_translate - a django app to perform OCR and translation of images.          #
+# Copyright (C) 2023-present Davide Grassano                                      #
+#                                                                                 #
+# This program is free software: you can redistribute it and/or modify            #
+# it under the terms of the GNU General Public License as published by            #
+# the Free Software Foundation, either version 3 of the License.                  #
+#                                                                                 #
+# This program is distributed in the hope that it will be useful,                 #
+# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
+# GNU General Public License for more details.                                    #
+#                                                                                 #
+# You should have received a copy of the GNU General Public License               #
+# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
+#                                                                                 #
+# Home: https://github.com/Crivella/ocr_translate                                 #
+###################################################################################
+"""Django models for the ocr_translate app."""
+from django.db import models
+
+LANG_LENGTH = 32
+
+class OptionDict(models.Model):
+    """Dictionary of options for OCR and translation"""
+    options = models.JSONField(unique=True)
+
+    def __str__(self):
+        return str(self.options)
+
+class Language(models.Model):
+    """Language used for translation"""
+    name = models.CharField(max_length=64, unique=True)
+    iso1 = models.CharField(max_length=8, unique=True)
+    iso2b = models.CharField(max_length=8, unique=True)
+    iso2t = models.CharField(max_length=8, unique=True)
+    iso3 = models.CharField(max_length=32, unique=True)
+
+    easyocr = models.CharField(max_length=32, null=True)
+    tesseract = models.CharField(max_length=32, null=True)
+    facebookM2M = models.CharField(max_length=32, null=True)
+
+    break_chars = models.CharField(max_length=512, null=True)
+    ignore_chars = models.CharField(max_length=512, null=True)
+
+    def __str__(self):
+        return str(self.iso1)
+
+class OCRModel(models.Model):
+    """OCR model using hugging space naming convention"""
+    name = models.CharField(max_length=128)
+    languages = models.ManyToManyField(Language, related_name='ocr_models')
+
+    language_format = models.CharField(max_length=32, null=True)
+
+    def __str__(self):
+        return str(self.name)
+
+class OCRBoxModel(models.Model):
+    """OCR model for bounding boxes"""
+    name = models.CharField(max_length=128)
+    languages = models.ManyToManyField(Language, related_name='box_models')
+
+    language_format = models.CharField(max_length=32, null=True)
+
+    def __str__(self):
+        return str(self.name)
+
+class TSLModel(models.Model):
+    """Translation models using hugging space naming convention"""
+    name = models.CharField(max_length=128)
+    src_languages = models.ManyToManyField(Language, related_name='tsl_models_src')
+    dst_languages = models.ManyToManyField(Language, related_name='tsl_models_dst')
+
+    language_format = models.CharField(max_length=32, null=True)
+
+    def __str__(self):
+        return str(self.name)
+
+class Image(models.Model):
+    """Image registered as the md5 of the uploaded file"""
+    md5 = models.CharField(max_length=32, unique=True)
+
+class BBox(models.Model):
+    """Bounding box of a text in an image"""
+    l = models.IntegerField(null=False)
+    b = models.IntegerField(null=False)
+    r = models.IntegerField(null=False)
+    t = models.IntegerField(null=False)
+
+    image = models.ForeignKey(Image, on_delete=models.CASCADE, related_name='bboxes')
+    from_ocr = models.ForeignKey('OCRBoxRun', on_delete=models.CASCADE, related_name='result')
+
+    @property
+    def lbrt(self):
+        """Return the bounding box as a tuple of (left, bottom, right, top)"""
+        return self.l, self.b, self.r, self.t
+
+    def __str__(self):
+        return f'{self.lbrt}'
+
+class Text(models.Model):
+    """Text extracted from an image or translated from another text"""
+    text = models.TextField()
+    # lang = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='texts')
+
+class OCRBoxRun(models.Model):
+    """OCR run on an image using a specific model"""
+    options = models.ForeignKey(OptionDict, on_delete=models.CASCADE, related_name='ocr_box_options')
+
+    lang_src = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='box_src')
+
+    image = models.ForeignKey(Image, on_delete=models.CASCADE, related_name='to_box')
+    model = models.ForeignKey(OCRBoxModel, on_delete=models.CASCADE, related_name='box_runs')
+    # result = models.ForeignKey(BBox, on_delete=models.CASCADE, related_name='from_ocr')
+
+class OCRRun(models.Model):
+    """OCR run on an image using a specific model"""
+    options = models.ForeignKey(OptionDict, on_delete=models.CASCADE, related_name='ocr_options')
+
+    lang_src = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='ocr_src')
+
+    # image = models.ForeignKey(Image, on_delete=models.CASCADE, related_name='to_ocr')
+    bbox = models.ForeignKey(BBox, on_delete=models.CASCADE, related_name='to_ocr')
+    model = models.ForeignKey(OCRModel, on_delete=models.CASCADE, related_name='ocr_runs')
+    result = models.ForeignKey(Text, on_delete=models.CASCADE, related_name='from_ocr')
+
+class TranslationRun(models.Model):
+    """Translation run on a text using a specific model"""
+    options = models.ForeignKey(OptionDict, on_delete=models.CASCADE, related_name='trans_options')
+
+    lang_src = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='trans_src')
+    lang_dst = models.ForeignKey(Language, on_delete=models.CASCADE, related_name='trans_dst')
+
+    text = models.ForeignKey(Text, on_delete=models.CASCADE, related_name='to_trans')
+    model = models.ForeignKey(TSLModel, on_delete=models.CASCADE, related_name='tsl_runs')
+    result = models.ForeignKey(Text, on_delete=models.CASCADE, related_name='from_trans')
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/queues.py` & `django_ocr_translate-0.1.3/ocr_translate/queues.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-###################################################################################
-# ocr_translate - a django app to perform OCR and translation of images.          #
-# Copyright (C) 2023-present Davide Grassano                                      #
-#                                                                                 #
-# This program is free software: you can redistribute it and/or modify            #
-# it under the terms of the GNU General Public License as published by            #
-# the Free Software Foundation, either version 3 of the License.                  #
-#                                                                                 #
-# This program is distributed in the hope that it will be useful,                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
-# GNU General Public License for more details.                                    #
-#                                                                                 #
-# You should have received a copy of the GNU General Public License               #
-# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
-#                                                                                 #
-# Home: https://github.com/Crivella/ocr_translate                                 #
-###################################################################################
-import os
-
-from .messaging import WorkerMessageQueue
-
-num_main_workers = int(os.environ.get('NUM_MAIN_WORKERS', 4))
-num_box_workers = int(os.environ.get('NUM_BOX_WORKERS', 1))
-num_ocr_workers = int(os.environ.get('NUM_OCR_WORKERS', 1))
-num_tsl_workers = int(os.environ.get('NUM_TSL_WORKERS', 1))
-
-main_queue = WorkerMessageQueue(num_workers=num_main_workers)
-box_queue = WorkerMessageQueue(num_workers=num_box_workers)
-ocr_queue = WorkerMessageQueue(num_workers=num_ocr_workers)
-tsl_queue = WorkerMessageQueue(
-    num_workers=num_tsl_workers,
-    allow_batching=True,
-    # batch_timeout=15,
-    batch_args= (0,)
-    )
-
-main_queue.start_workers()
-box_queue.start_workers()
-ocr_queue.start_workers()
-tsl_queue.start_workers()
-
+###################################################################################
+# ocr_translate - a django app to perform OCR and translation of images.          #
+# Copyright (C) 2023-present Davide Grassano                                      #
+#                                                                                 #
+# This program is free software: you can redistribute it and/or modify            #
+# it under the terms of the GNU General Public License as published by            #
+# the Free Software Foundation, either version 3 of the License.                  #
+#                                                                                 #
+# This program is distributed in the hope that it will be useful,                 #
+# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
+# GNU General Public License for more details.                                    #
+#                                                                                 #
+# You should have received a copy of the GNU General Public License               #
+# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
+#                                                                                 #
+# Home: https://github.com/Crivella/ocr_translate                                 #
+###################################################################################
+"""Queues definition for the ocr_translate app."""
+import os
+
+from .messaging import WorkerMessageQueue
+
+num_main_workers = int(os.environ.get('NUM_MAIN_WORKERS', 4))
+num_box_workers = int(os.environ.get('NUM_BOX_WORKERS', 1))
+num_ocr_workers = int(os.environ.get('NUM_OCR_WORKERS', 1))
+num_tsl_workers = int(os.environ.get('NUM_TSL_WORKERS', 1))
+
+main_queue = WorkerMessageQueue(num_workers=num_main_workers)
+box_queue = WorkerMessageQueue(num_workers=num_box_workers)
+ocr_queue = WorkerMessageQueue(num_workers=num_ocr_workers)
+tsl_queue = WorkerMessageQueue(
+    num_workers=num_tsl_workers,
+    allow_batching=True,
+    # batch_timeout=15,
+    batch_args= (0,)
+    )
+
+main_queue.start_workers()
+box_queue.start_workers()
+ocr_queue.start_workers()
+tsl_queue.start_workers()
```

### Comparing `django_ocr_translate-0.1.2/ocr_translate/views.py` & `django_ocr_translate-0.1.3/ocr_translate/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,275 +1,338 @@
-###################################################################################
-# ocr_translate - a django app to perform OCR and translation of images.          #
-# Copyright (C) 2023-present Davide Grassano                                      #
-#                                                                                 #
-# This program is free software: you can redistribute it and/or modify            #
-# it under the terms of the GNU General Public License as published by            #
-# the Free Software Foundation, either version 3 of the License.                  #
-#                                                                                 #
-# This program is distributed in the hope that it will be useful,                 #
-# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
-# GNU General Public License for more details.                                    #
-#                                                                                 #
-# You should have received a copy of the GNU General Public License               #
-# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
-#                                                                                 #
-# Home: https://github.com/Crivella/ocr_translate                                 #
-###################################################################################
-import base64
-import hashlib
-import io
-import json
-import logging
-
-import numpy as np
-from django.db.models import Count
-from django.http import HttpRequest, JsonResponse
-from django.middleware import csrf
-from django.views.decorators.csrf import csrf_exempt
-from PIL import Image
-
-from . import models as m
-from .OCR_TSL import ocr_tsl_pipeline_lazy, ocr_tsl_pipeline_work
-from .OCR_TSL.box import get_box_model, load_box_model, unload_box_model
-from .OCR_TSL.lang import (get_lang_dst, get_lang_src, load_lang_dst,
-                           load_lang_src)
-from .OCR_TSL.ocr import get_ocr_model, load_ocr_model, unload_ocr_model
-from .OCR_TSL.tsl import (get_tsl_model, load_tsl_model, tsl_run,
-                          unload_tsl_model)
-from .queues import main_queue as q
-
-logger = logging.getLogger('ocr.general')
-
-
-def post_data_converter(request: HttpRequest) -> dict:
-    if request.content_type == 'application/json':
-        return json.loads(request.body)
-    else:
-        raise ValueError('invalid content type')
-
-
-def handshake(request: HttpRequest) -> JsonResponse:
-    # import_models()
-    if not request.method == 'GET':
-        return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
-    
-    csrf.get_token(request)
-    
-    logger.debug(f'Handshake: {str(get_ocr_model())}, {str(get_tsl_model())}')
-    lang_src = get_lang_src()
-    lang_dst = get_lang_dst()
-
-    languages = m.Language.objects.annotate(count=Count('trans_src')+Count('trans_dst')).order_by('-count')
-    box_models = m.OCRBoxModel.objects.annotate(count=Count('box_runs')).order_by('-count')
-    ocr_models = m.OCRModel.objects.annotate(count=Count('ocr_runs')).order_by('-count')
-    tsl_models = m.TSLModel.objects.annotate(count=Count('tsl_runs')).order_by('-count')
-
-    if not lang_src is None:
-        box_models = box_models.filter(languages=lang_src)
-        ocr_models = ocr_models.filter(languages=lang_src)
-        if not lang_dst is None:
-            tsl_models = tsl_models.filter(
-                src_languages=lang_src,
-                dst_languages=lang_dst,
-                )
-            
-    box_model = get_box_model() or ''
-    ocr_model = get_ocr_model() or ''
-    tsl_model = get_tsl_model() or ''
-
-    lang_src = lang_src or ''
-    lang_dst = lang_dst or ''
-
-    return JsonResponse({
-        'Languages': [str(_) for _ in languages],
-        'BOXModels': [str(_) for _ in box_models],
-        'OCRModels': [str(_) for _ in ocr_models],
-        'TSLModels': [str(_) for _ in tsl_models],
-
-        'box_selected': str(box_model), 
-        'ocr_selected': str(ocr_model),
-        'tsl_selected': str(tsl_model), 
-        'lang_src': str(lang_src),
-        'lang_dst': str(lang_dst),
-        })
-
-@csrf_exempt
-def load_models(request: HttpRequest) -> JsonResponse:
-    if request.method == 'POST':
-        try:
-            data = post_data_converter(request)
-        except ValueError as e:
-            return JsonResponse({'error': 'invalid content type'}, status=400)
-
-        logger.info('LOAD MODELS', data)
-        logger.debug(data)
-        
-        box_model_id = data.get('box_model_id', None)
-        ocr_model_id = data.get('ocr_model_id', None)
-        tsl_model_id = data.get('tsl_model_id', None)
-
-        try:
-            if not box_model_id is None and not box_model_id == '':
-                load_box_model(box_model_id)
-            if not ocr_model_id is None and not ocr_model_id == '':
-                load_ocr_model(ocr_model_id)
-            if not tsl_model_id is None and not tsl_model_id == '':
-                load_tsl_model(tsl_model_id)
-        except Exception as e:
-            return JsonResponse({'error': str(e)}, status=400)
-        
-        return JsonResponse({})
-    return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
-
-@csrf_exempt
-def set_lang(request: HttpRequest) -> JsonResponse:
-    if request.method == 'POST':
-        try:
-            data = post_data_converter(request)
-        except ValueError as e:
-            return JsonResponse({'error': 'invalid content type'}, status=400)
-        logger.info('SET LANG', data)
-        
-        lang_src = data.get('lang_src', None)
-        lang_dst = data.get('lang_dst', None)
-        if lang_src is None:
-            return JsonResponse({'error': 'no lang_src'}, status=400)
-        if lang_dst is None:
-            return JsonResponse({'error': 'no lang_dst'}, status=400)
-
-        old_src = get_lang_src()
-        old_dst = get_lang_dst()
-        try:
-            load_lang_src(lang_src)
-            load_lang_dst(lang_dst)
-        except Exception as e:
-            return JsonResponse({'error': str(e)}, status=400)
-        new_src = get_lang_src()
-        new_dst = get_lang_dst()
-
-        c1 = old_src != new_src
-        c2 = old_dst != new_dst
-        if c1 or c2:
-            tsl_model = get_tsl_model()
-            if not tsl_model is None and (new_src not in tsl_model.src_languages.all() or new_dst not in tsl_model.dst_languages.all()):
-                unload_tsl_model()
-        if c1:
-            box_model = get_box_model()
-            ocr_model = get_ocr_model()
-            if not box_model is None and (new_src not in box_model.languages.all()):
-                unload_box_model()
-            if not ocr_model is None and (new_src not in ocr_model.languages.all()):
-                unload_ocr_model()
-        if c2:
-            pass
-        
-        return JsonResponse({})
-    return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
-
-@csrf_exempt
-def run_tsl(request: HttpRequest) -> JsonResponse:
-    if request.method != 'POST':
-        return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
-    
-    try:
-        data = post_data_converter(request)
-    except ValueError as e:
-        return JsonResponse({'error': 'invalid content type'}, status=400)
-    
-    text = data.get('text', None)
-    if text is None:
-        return JsonResponse({'error': 'no text'}, status=400)
-    
-    src_obj, _ = m.Text.objects.get_or_create(text=text)
-    dst_obj = tsl_run(src_obj, get_lang_src(), get_lang_dst())
-    dst_obj = next(dst_obj)
-
-    return JsonResponse({
-        'text': dst_obj.text,
-        })
-
-@csrf_exempt
-def run_ocrtsl(request: HttpRequest) -> JsonResponse:
-    if request.method == 'POST':
-        try:
-            data = post_data_converter(request)
-        except ValueError as e:
-            return JsonResponse({'error': 'invalid content type'}, status=400)
-        
-        b64 = data.get('contents', None)
-        md5 = data.get('md5')
-        frc = data.get('force', False)
-        opt = data.get('options', {})
-
-        if b64 is None:
-            logger.info('No contents, trying to lazyload')
-            if frc:
-                return JsonResponse({'error': 'Cannot force ocr without contents'}, status=400)
-            try:
-                res = ocr_tsl_pipeline_lazy(md5, options=opt)
-            except ValueError:
-                return JsonResponse({'error': 'Failed to lazyload ocr'}, status=406)
-        else:
-            bin = base64.b64decode(b64)
-            # Doing md5 on the base64 to have consistency with the JS generate one
-            # Can't find a way to run md5 on the binary in JS (the blob does not work)
-            if md5 != hashlib.md5(b64.encode('utf-8')).hexdigest():
-                return JsonResponse({'error': 'md5 mismatch'}, status=400)
-            logger.debug(f'md5 {md5} <- {len(bin)} bytes')
-
-            img = Image.open(io.BytesIO(bin))
-            # Needed to make sure the image is loaded synchronously before going forward
-            # Enforce thread safety. Maybe there is a way to do it without numpy?
-            np.array(img)
-
-            # Check if same request is already in queue. If yes attach listener to it
-            lang_src = get_lang_src()
-            lang_dst = get_lang_dst()
-            box_model = get_box_model()
-            ocr_model = get_ocr_model()
-            tsl_model = get_tsl_model()
-            msg = q.put(
-                id = (md5, lang_src.id, lang_dst.id, box_model.id, ocr_model.id, tsl_model.id),
-                msg = {
-                    'args': (img, md5),
-                    'kwargs': {'force': frc, 'options': opt},
-                },
-                handler = ocr_tsl_pipeline_work,
-            )
-
-            res = msg.response()
-
-
-        return JsonResponse({
-            'test': 'POST',
-            'result': res,
-            })
-    return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
-
-@csrf_exempt
-def get_translations(request: HttpRequest) -> JsonResponse:
-    if request.method != 'GET':
-        return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
-
-    text = request.GET.get('text', None)
-
-    if text is None:
-        return JsonResponse({'error': 'no text'}, status=400)
-    
-    text_obj = m.Text.objects.filter(text=text).first()
-    if text_obj is None:
-        return JsonResponse({'error': 'text not found'}, status=404)
-    
-    translations = text_obj.to_trans.filter(
-        lang_src=get_lang_src(),
-        lang_dst=get_lang_dst(),
-        )
-    return JsonResponse({
-        'translations': [{
-            'model': str(_.model),
-            'text': _.result.text,
-            } for _ in translations],
-        })
-
-
+###################################################################################
+# ocr_translate - a django app to perform OCR and translation of images.          #
+# Copyright (C) 2023-present Davide Grassano                                      #
+#                                                                                 #
+# This program is free software: you can redistribute it and/or modify            #
+# it under the terms of the GNU General Public License as published by            #
+# the Free Software Foundation, either version 3 of the License.                  #
+#                                                                                 #
+# This program is distributed in the hope that it will be useful,                 #
+# but WITHOUT ANY WARRANTY; without even the implied warranty of                  #
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                   #
+# GNU General Public License for more details.                                    #
+#                                                                                 #
+# You should have received a copy of the GNU General Public License               #
+# along with this program.  If not, see {http://www.gnu.org/licenses/}.           #
+#                                                                                 #
+# Home: https://github.com/Crivella/ocr_translate                                 #
+###################################################################################
+"""Django views for the ocr_translate app."""
+# pylint: disable=too-many-return-statements
+import base64
+import hashlib
+import io
+import json
+import logging
+
+import numpy as np
+from django.db.models import Count
+from django.http import HttpRequest, JsonResponse
+from django.middleware import csrf
+from django.views.decorators.csrf import csrf_exempt
+from PIL import Image
+
+from . import models as m
+from .ocr_tsl.box import get_box_model, load_box_model, unload_box_model
+from .ocr_tsl.full import ocr_tsl_pipeline_lazy, ocr_tsl_pipeline_work
+from .ocr_tsl.lang import (get_lang_dst, get_lang_src, load_lang_dst,
+                           load_lang_src)
+from .ocr_tsl.ocr import get_ocr_model, load_ocr_model, unload_ocr_model
+from .ocr_tsl.tsl import (get_tsl_model, load_tsl_model, tsl_run,
+                          unload_tsl_model)
+from .queues import main_queue as q
+
+logger = logging.getLogger('ocr.general')
+
+
+def post_data_converter(request: HttpRequest) -> dict:
+    """Convert POST data to a dict."""
+    if request.content_type == 'application/json':
+        return json.loads(request.body)
+
+    raise ValueError('invalid content type')
+
+
+def handshake(request: HttpRequest) -> JsonResponse:
+    """Handshake with the client."""
+    if not request.method == 'GET':
+        return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
+
+    csrf.get_token(request)
+
+    logger.debug(f'Handshake: {str(get_ocr_model())}, {str(get_tsl_model())}')
+    lang_src = get_lang_src()
+    lang_dst = get_lang_dst()
+
+    languages = m.Language.objects.annotate(count=Count('trans_src')+Count('trans_dst')).order_by('-count')
+    box_models = m.OCRBoxModel.objects.annotate(count=Count('box_runs')).order_by('-count')
+    ocr_models = m.OCRModel.objects.annotate(count=Count('ocr_runs')).order_by('-count')
+    tsl_models = m.TSLModel.objects.annotate(count=Count('tsl_runs')).order_by('-count')
+
+    if not lang_src is None:
+        box_models = box_models.filter(languages=lang_src)
+        ocr_models = ocr_models.filter(languages=lang_src)
+        if not lang_dst is None:
+            tsl_models = tsl_models.filter(
+                src_languages=lang_src,
+                dst_languages=lang_dst,
+                )
+
+    box_model = get_box_model() or ''
+    ocr_model = get_ocr_model() or ''
+    tsl_model = get_tsl_model() or ''
+
+    lang_src = lang_src or ''
+    lang_dst = lang_dst or ''
+
+    return JsonResponse({
+        'Languages': [str(_) for _ in languages],
+        'BOXModels': [str(_) for _ in box_models],
+        'OCRModels': [str(_) for _ in ocr_models],
+        'TSLModels': [str(_) for _ in tsl_models],
+
+        'box_selected': str(box_model),
+        'ocr_selected': str(ocr_model),
+        'tsl_selected': str(tsl_model),
+        'lang_src': str(lang_src),
+        'lang_dst': str(lang_dst),
+        })
+
+@csrf_exempt
+def set_models(request: HttpRequest) -> JsonResponse:
+    """Handle a POST request to load models.
+    Expected data:
+    {
+        'box_model_id': 'id',
+        'ocr_model_id': 'id',
+        'tsl_model_id': 'id',
+    }
+    """
+    if request.method == 'POST':
+        try:
+            data = post_data_converter(request)
+        except ValueError:
+            return JsonResponse({'error': 'invalid content type'}, status=400)
+
+        logger.info(f'LOAD MODELS: {data}')
+
+        box_model_id = data.pop('box_model_id', None)
+        ocr_model_id = data.pop('ocr_model_id', None)
+        tsl_model_id = data.pop('tsl_model_id', None)
+
+        if len(data) > 0:
+            return JsonResponse({'error': f'invalid data: {data}'}, status=400)
+
+        try:
+            if not box_model_id is None and not box_model_id == '':
+                load_box_model(box_model_id)
+            if not ocr_model_id is None and not ocr_model_id == '':
+                load_ocr_model(ocr_model_id)
+            if not tsl_model_id is None and not tsl_model_id == '':
+                load_tsl_model(tsl_model_id)
+        except Exception as exc:
+            return JsonResponse({'error': str(exc)}, status=400)
+
+        return JsonResponse({})
+    return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
+
+@csrf_exempt
+def set_lang(request: HttpRequest) -> JsonResponse:
+    """Handle a POST request to set languages.
+    Expected data:
+    {
+        'lang_src': 'id',
+        'lang_dst': 'id',
+    }
+    """
+    if request.method != 'POST':
+        return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
+
+    try:
+        data = post_data_converter(request)
+    except ValueError:
+        return JsonResponse({'error': 'invalid content type'}, status=400)
+    logger.info(f'SET LANG: {data}')
+
+    lang_src = data.pop('lang_src', None)
+    lang_dst = data.pop('lang_dst', None)
+    if lang_src is None:
+        return JsonResponse({'error': 'no lang_src'}, status=400)
+    if lang_dst is None:
+        return JsonResponse({'error': 'no lang_dst'}, status=400)
+    if len(data) > 0:
+        return JsonResponse({'error': f'invalid data: {data}'}, status=400)
+
+    old_src = get_lang_src()
+    old_dst = get_lang_dst()
+    try:
+        load_lang_src(lang_src)
+        load_lang_dst(lang_dst)
+    except Exception as exc:
+        return JsonResponse({'error': str(exc)}, status=400)
+    new_src = get_lang_src()
+    new_dst = get_lang_dst()
+
+    check1 = old_src != new_src
+    check2 = old_dst != new_dst
+    if check1 or check2:
+        tsl_model = get_tsl_model()
+        if (
+            not tsl_model is None and
+            (
+                new_src not in tsl_model.src_languages.all() or
+                new_dst not in tsl_model.dst_languages.all()
+            )):
+            unload_tsl_model()
+    if check1:
+        box_model = get_box_model()
+        ocr_model = get_ocr_model()
+        if not box_model is None and (new_src not in box_model.languages.all()):
+            unload_box_model()
+        if not ocr_model is None and (new_src not in ocr_model.languages.all()):
+            unload_ocr_model()
+    # if check2:
+    #     pass
+
+    return JsonResponse({})
+
+@csrf_exempt
+def run_tsl(request: HttpRequest) -> JsonResponse:
+    """Handle a POST request to run translation.
+    Expected data:
+    {
+        'text': 'text',
+    }
+    """
+    if request.method != 'POST':
+        return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
+
+    try:
+        data = post_data_converter(request)
+    except ValueError:
+        return JsonResponse({'error': 'invalid content type'}, status=400)
+
+    text = data.pop('text', None)
+    if text is None:
+        return JsonResponse({'error': 'no text'}, status=400)
+    if len(data) > 0:
+        return JsonResponse({'error': f'invalid data: {data}'}, status=400)
+
+
+    src_obj, _ = m.Text.objects.get_or_create(text=text)
+    dst_obj = tsl_run(src_obj, get_lang_src(), get_lang_dst())
+    dst_obj = next(dst_obj)
+
+    return JsonResponse({
+        'text': dst_obj.text,
+        })
+
+@csrf_exempt
+def run_ocrtsl(request: HttpRequest) -> JsonResponse:
+    """Handle a POST request to run OCR and translation.
+    Expected data:
+    {
+        'contents': 'base64',
+        'md5': 'md5',
+        'force': 'bool',
+        'options': 'dict',
+    }
+    """
+    if request.method == 'POST':
+        try:
+            data = post_data_converter(request)
+        except ValueError:
+            return JsonResponse({'error': 'invalid content type'}, status=400)
+
+        b64 = data.pop('contents', None)
+        md5 = data.pop('md5', None)
+        frc = data.pop('force', False)
+        opt = data.pop('options', {})
+
+        if md5 is None:
+            return JsonResponse({'error': 'no md5'}, status=400)
+        if len(data) > 0:
+            return JsonResponse({'error': f'invalid data: {data}'}, status=400)
+
+        if b64 is None:
+            logger.info('No contents, trying to lazyload')
+            if frc:
+                return JsonResponse({'error': 'Cannot force ocr without contents'}, status=400)
+            try:
+                res = ocr_tsl_pipeline_lazy(md5, options=opt)
+            except ValueError:
+                return JsonResponse({'error': 'Failed to lazyload ocr'}, status=406)
+        else:
+            binary = base64.b64decode(b64)
+            # Doing md5 on the base64 to have consistency with the JS generate one
+            # Can't find a way to run md5 on the binary in JS (the blob does not work)
+            if md5 != hashlib.md5(b64.encode('utf-8')).hexdigest():
+                return JsonResponse({'error': 'md5 mismatch'}, status=400)
+            logger.debug(f'md5 {md5} <- {len(binary)} bytes')
+
+            img = Image.open(io.BytesIO(binary))
+            # Needed to make sure the image is loaded synchronously before going forward
+            # Enforce thread safety. Maybe there is a way to do it without numpy?
+            np.array(img)
+
+            # Check if same request is already in queue. If yes attach listener to it
+            lang_src = get_lang_src()
+            lang_dst = get_lang_dst()
+            box_model = get_box_model()
+            ocr_model = get_ocr_model()
+            tsl_model = get_tsl_model()
+
+            try:
+                id_ = (md5, lang_src.id, lang_dst.id, box_model.id, ocr_model.id, tsl_model.id)
+            except AttributeError:
+                return JsonResponse({'error': 'No models selected'}, status=400)
+
+            msg = q.put(
+                id_ = id_,
+                msg = {
+                    'args': (img, md5),
+                    'kwargs': {'force': frc, 'options': opt},
+                },
+                handler = ocr_tsl_pipeline_work,
+            )
+
+            res = msg.response()
+
+
+        return JsonResponse({
+            'result': res,
+            })
+    return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
+
+@csrf_exempt
+def get_translations(request: HttpRequest) -> JsonResponse:
+    """Handle a GET request to get translations.
+    Expected parameters:
+    {
+        'text': 'text',
+    }
+    """
+    if request.method != 'GET':
+        return JsonResponse({'error': f'{request.method} not allowed'}, status=405)
+
+    params = request.GET.dict()
+    text = params.pop('text', None)
+
+    if len(params) > 0:
+        return JsonResponse({'error': f'invalid data: {params}'}, status=400)
+    if text is None:
+        return JsonResponse({'error': 'no text'}, status=400)
+
+    text_obj = m.Text.objects.filter(text=text).first()
+    if text_obj is None:
+        return JsonResponse({'error': 'text not found'}, status=404)
+
+    translations = text_obj.to_trans.filter(
+        lang_src=get_lang_src(),
+        lang_dst=get_lang_dst(),
+        )
+    return JsonResponse({
+        'translations': [{
+            'model': str(_.model),
+            'text': _.result.text,
+            } for _ in translations],
+        })
```

### Comparing `django_ocr_translate-0.1.2/pyproject.toml` & `django_ocr_translate-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,185 @@
-00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0a23  [build-system].#
-00000010: 2062 7569 6c64 2074 6865 2070 6163 6b61   build the packa
-00000020: 6765 2077 6974 6820 5b66 6c69 745d 2868  ge with [flit](h
-00000030: 7474 7073 3a2f 2f66 6c69 742e 7265 6164  ttps://flit.read
-00000040: 7468 6564 6f63 732e 696f 290a 7265 7175  thedocs.io).requ
-00000050: 6972 6573 203d 205b 2266 6c69 745f 636f  ires = ["flit_co
-00000060: 7265 203e 3d33 2e34 2c3c 3422 5d0a 6275  re >=3.4,<4"].bu
-00000070: 696c 642d 6261 636b 656e 6420 3d20 2266  ild-backend = "f
-00000080: 6c69 745f 636f 7265 2e62 7569 6c64 6170  lit_core.buildap
-00000090: 6922 0a0a 5b70 726f 6a65 6374 5d0a 2320  i"..[project].# 
-000000a0: 5365 6520 6874 7470 733a 2f2f 7777 772e  See https://www.
-000000b0: 7079 7468 6f6e 2e6f 7267 2f64 6576 2f70  python.org/dev/p
-000000c0: 6570 732f 7065 702d 3036 3231 2f0a 6e61  eps/pep-0621/.na
-000000d0: 6d65 203d 2022 646a 616e 676f 2d6f 6372  me = "django-ocr
-000000e0: 5f74 7261 6e73 6c61 7465 220a 6479 6e61  _translate".dyna
-000000f0: 6d69 6320 3d20 5b22 7665 7273 696f 6e22  mic = ["version"
-00000100: 5d20 2320 7265 6164 2066 726f 6d20 6f63  ] # read from oc
-00000110: 725f 7472 616e 736c 6174 652f 5f5f 696e  r_translate/__in
-00000120: 6974 5f5f 2e70 790a 6465 7363 7269 7074  it__.py.descript
-00000130: 696f 6e20 3d20 2244 6a61 6e67 6f20 6170  ion = "Django ap
-00000140: 7020 666f 7220 4f43 5220 616e 6420 7472  p for OCR and tr
-00000150: 616e 736c 6174 696f 6e22 0a61 7574 686f  anslation".autho
-00000160: 7273 203d 205b 0a20 2020 207b 206e 616d  rs = [.    { nam
-00000170: 6520 3d20 2244 6176 6964 6520 4772 6173  e = "Davide Gras
-00000180: 7361 6e6f 2220 7d2c 0a5d 0a72 6561 646d  sano" },.].readm
-00000190: 6520 3d20 2252 4541 444d 452e 6d64 220a  e = "README.md".
-000001a0: 6c69 6365 6e73 6520 3d20 7b20 6669 6c65  license = { file
-000001b0: 203d 2022 4c49 4345 4e53 452e 7478 7422   = "LICENSE.txt"
-000001c0: 207d 0a63 6c61 7373 6966 6965 7273 203d   }.classifiers =
-000001d0: 205b 0a20 2020 2022 4465 7665 6c6f 706d   [.    "Developm
-000001e0: 656e 7420 5374 6174 7573 203a 3a20 3220  ent Status :: 2 
-000001f0: 2d20 5072 652d 416c 7068 6122 2c0a 2020  - Pre-Alpha",.  
-00000200: 2020 2246 7261 6d65 776f 726b 203a 3a20    "Framework :: 
-00000210: 446a 616e 676f 222c 0a20 2020 2022 4c69  Django",.    "Li
-00000220: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000230: 726f 7665 6420 3a3a 2047 4e55 2047 656e  roved :: GNU Gen
-00000240: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00000250: 6e73 6520 7633 2028 4750 4c76 3329 222c  nse v3 (GPLv3)",
-00000260: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
-00000270: 5379 7374 656d 203a 3a20 4d69 6372 6f73  System :: Micros
-00000280: 6f66 7420 3a3a 2057 696e 646f 7773 222c  oft :: Windows",
-00000290: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
-000002a0: 5379 7374 656d 203a 3a20 504f 5349 5820  System :: POSIX 
-000002b0: 3a3a 204c 696e 7578 222c 0a20 2020 2022  :: Linux",.    "
-000002c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002d0: 7561 6765 203a 3a20 5079 7468 6f6e 222c  uage :: Python",
-000002e0: 0a20 2020 2022 5072 6f67 7261 6d6d 696e  .    "Programmin
-000002f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000300: 7468 6f6e 203a 3a20 332e 3130 222c 0a20  thon :: 3.10",. 
-00000310: 2020 2022 4e61 7475 7261 6c20 4c61 6e67     "Natural Lang
-00000320: 7561 6765 203a 3a20 456e 676c 6973 6822  uage :: English"
-00000330: 2c0a 2020 2020 2254 6f70 6963 203a 3a20  ,.    "Topic :: 
-00000340: 4d75 6c74 696d 6564 6961 203a 3a20 4772  Multimedia :: Gr
-00000350: 6170 6869 6373 222c 0a20 2020 2022 546f  aphics",.    "To
-00000360: 7069 6320 3a3a 2044 6174 6162 6173 6520  pic :: Database 
-00000370: 3a3a 2044 6174 6162 6173 6520 456e 6769  :: Database Engi
-00000380: 6e65 732f 5365 7276 6572 7322 2c0a 2020  nes/Servers",.  
-00000390: 2020 2254 6f70 6963 203a 3a20 5465 7874    "Topic :: Text
-000003a0: 2050 726f 6365 7373 696e 6720 3a3a 204c   Processing :: L
-000003b0: 696e 6775 6973 7469 6322 2c0a 2020 2020  inguistic",.    
-000003c0: 2249 6e74 656e 6465 6420 4175 6469 656e  "Intended Audien
-000003d0: 6365 203a 3a20 456e 6420 5573 6572 732f  ce :: End Users/
-000003e0: 4465 736b 746f 7022 2c0a 5d0a 6b65 7977  Desktop",.].keyw
-000003f0: 6f72 6473 203d 205b 2264 6a61 6e67 6f22  ords = ["django"
-00000400: 2c20 226f 6372 222c 2022 7472 616e 736c  , "ocr", "transl
-00000410: 6174 696f 6e22 5d0a 7265 7175 6972 6573  ation"].requires
-00000420: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
-00000430: 3022 0a64 6570 656e 6465 6e63 6965 7320  0".dependencies 
-00000440: 3d20 5b0a 2020 2020 2272 6567 6578 3d3d  = [.    "regex==
-00000450: 3230 3233 2e36 2e33 222c 0a20 2020 2022  2023.6.3",.    "
-00000460: 7265 7175 6573 7473 3d3d 322e 3331 2e30  requests==2.31.0
-00000470: 222c 0a20 2020 2022 446a 616e 676f 3d3d  ",.    "Django==
-00000480: 342e 322e 3222 2c0a 2020 2020 2250 696c  4.2.2",.    "Pil
-00000490: 6c6f 773d 3d39 2e35 2e30 222c 0a20 2020  low==9.5.0",.   
-000004a0: 2022 6f70 656e 6376 2d70 7974 686f 6e2d   "opencv-python-
-000004b0: 6865 6164 6c65 7373 3d3d 342e 382e 302e  headless==4.8.0.
-000004c0: 3734 222c 0a0a 2020 2020 2274 6f72 6368  74",..    "torch
-000004d0: 3d3d 322e 302e 3122 2c0a 2020 2020 2274  ==2.0.1",.    "t
-000004e0: 6f72 6368 7669 7369 6f6e 3d3d 302e 3135  orchvision==0.15
-000004f0: 2e32 222c 0a0a 2020 2020 2274 7261 6e73  .2",..    "trans
-00000500: 666f 726d 6572 733d 3d34 2e33 302e 3222  formers==4.30.2"
-00000510: 2c0a 2020 2020 2265 6173 796f 6372 3d3d  ,.    "easyocr==
-00000520: 312e 372e 3022 2c0a 2020 2020 2270 7974  1.7.0",.    "pyt
-00000530: 6573 7365 7261 6374 3d3d 302e 332e 3130  esseract==0.3.10
-00000540: 222c 0a20 2020 2022 6675 6761 7368 693d  ",.    "fugashi=
-00000550: 3d31 2e32 2e31 222c 0a20 2020 2022 756e  =1.2.1",.    "un
-00000560: 6964 6963 2d6c 6974 653d 3d31 2e30 2e38  idic-lite==1.0.8
-00000570: 222c 0a20 2020 2022 7361 6372 656d 6f73  ",.    "sacremos
-00000580: 6573 3d3d 302e 302e 3533 222c 0a20 2020  es==0.0.53",.   
-00000590: 2022 7361 6665 7465 6e73 6f72 733d 3d30   "safetensors==0
-000005a0: 2e33 2e31 222c 0a20 2020 2022 7365 6e74  .3.1",.    "sent
-000005b0: 656e 6365 7069 6563 653d 3d30 2e31 2e39  encepiece==0.1.9
-000005c0: 3922 2c0a 5d0a 0a5b 7072 6f6a 6563 742e  9",.]..[project.
-000005d0: 7572 6c73 5d0a 536f 7572 6365 203d 2022  urls].Source = "
-000005e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000005f0: 6f6d 2f63 7269 7665 6c6c 612f 6f63 725f  om/crivella/ocr_
-00000600: 7472 616e 736c 6174 6522 0a23 2044 6f63  translate".# Doc
-00000610: 756d 656e 7461 7469 6f6e 203d 2022 6874  umentation = "ht
-00000620: 7470 733a 2f2f 6169 6964 612d 7761 6e6e  tps://aiida-wann
-00000630: 6965 7274 6f6f 6c73 2e72 6561 6474 6865  iertools.readthe
-00000640: 646f 6373 2e69 6f22 0a0a 5b70 726f 6a65  docs.io"..[proje
-00000650: 6374 2e6f 7074 696f 6e61 6c2d 6465 7065  ct.optional-depe
-00000660: 6e64 656e 6369 6573 5d0a 6d79 7371 6c20  ndencies].mysql 
-00000670: 3d20 5b0a 2020 2020 2270 796d 7973 716c  = [.    "pymysql
-00000680: 3d3d 312e 312e 3022 2c0a 5d0a 706f 7374  ==1.1.0",.].post
-00000690: 6772 6573 203d 205b 0a20 2020 2022 7073  gres = [.    "ps
-000006a0: 7963 6f70 675b 6269 6e61 7279 5d3d 3d33  ycopg[binary]==3
-000006b0: 2e31 2e39 222c 0a5d 0a23 2074 6573 7473  .1.9",.].# tests
-000006c0: 203d 205b 0a23 2020 2020 2022 7079 7465   = [.#     "pyte
-000006d0: 7374 222c 0a23 2020 2020 2022 7079 7465  st",.#     "pyte
-000006e0: 7374 2d63 6f76 222c 0a23 2020 2020 2022  st-cov",.#     "
-000006f0: 7079 7465 7374 2d72 6567 7265 7373 696f  pytest-regressio
-00000700: 6e73 7e3d 322e 3422 2c0a 2320 2020 2020  ns~=2.4",.#     
-00000710: 2270 7974 6573 742d 6461 7461 6469 727e  "pytest-datadir~
-00000720: 3d31 2e33 2e31 222c 0a23 2020 2020 2022  =1.3.1",.#     "
-00000730: 7067 7465 7374 7e3d 312e 332e 3122 0a23  pgtest~=1.3.1".#
-00000740: 205d 0a23 2070 7265 2d63 6f6d 6d69 7420   ].# pre-commit 
-00000750: 3d20 5b0a 2320 2020 2020 2270 7265 2d63  = [.#     "pre-c
-00000760: 6f6d 6d69 7422 2c0a 2320 2020 2020 2270  ommit",.#     "p
-00000770: 796c 696e 7422 2c0a 2320 2020 2020 2270  ylint",.#     "p
-00000780: 796c 696e 742d 7079 7465 7374 222c 0a23  ylint-pytest",.#
-00000790: 2020 2020 2022 7072 6f73 7065 6374 6f72       "prospector
-000007a0: 3e3d 312e 332e 3122 2c0a 2320 2020 2020  >=1.3.1",.#     
-000007b0: 2272 7561 6d65 6c2e 7961 6d6c 220a 2320  "ruamel.yaml".# 
-000007c0: 5d0a 0a5b 746f 6f6c 2e66 6c69 742e 6d6f  ]..[tool.flit.mo
-000007d0: 6475 6c65 5d0a 6e61 6d65 203d 2022 6f63  dule].name = "oc
-000007e0: 725f 7472 616e 736c 6174 6522 0a0a 5b74  r_translate"..[t
-000007f0: 6f6f 6c2e 666c 6974 2e73 6469 7374 5d0a  ool.flit.sdist].
-00000800: 6578 636c 7564 6520 3d20 5b0a 2020 2020  exclude = [.    
-00000810: 222e 6769 7469 676e 6f72 6522 2c0a 2020  ".gitignore",.  
-00000820: 2020 2244 6f63 6b65 7266 696c 6522 2c20    "Dockerfile", 
-00000830: 226e 6769 6e78 2e64 6566 6175 6c74 222c  "nginx.default",
-00000840: 2022 7374 6172 742d 7365 7276 6572 2e73   "start-server.s
-00000850: 6822 2c20 0a20 2020 2022 6d79 7369 7465  h", .    "mysite
-00000860: 2f22 2c20 226d 7973 6974 652f 2a22 2c20  /", "mysite/*", 
-00000870: 226d 616e 6167 652e 7079 220a 2020 2020  "manage.py".    
-00000880: 5d                                       ]
+00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
+00000010: 2320 6275 696c 6420 7468 6520 7061 636b  # build the pack
+00000020: 6167 6520 7769 7468 205b 666c 6974 5d28  age with [flit](
+00000030: 6874 7470 733a 2f2f 666c 6974 2e72 6561  https://flit.rea
+00000040: 6474 6865 646f 6373 2e69 6f29 0d0a 7265  dthedocs.io)..re
+00000050: 7175 6972 6573 203d 205b 2266 6c69 745f  quires = ["flit_
+00000060: 636f 7265 203e 3d33 2e34 2c3c 3422 5d0d  core >=3.4,<4"].
+00000070: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
+00000080: 2022 666c 6974 5f63 6f72 652e 6275 696c   "flit_core.buil
+00000090: 6461 7069 220d 0a0d 0a5b 7072 6f6a 6563  dapi"....[projec
+000000a0: 745d 0d0a 2320 5365 6520 6874 7470 733a  t]..# See https:
+000000b0: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+000000c0: 2f64 6576 2f70 6570 732f 7065 702d 3036  /dev/peps/pep-06
+000000d0: 3231 2f0d 0a6e 616d 6520 3d20 2264 6a61  21/..name = "dja
+000000e0: 6e67 6f2d 6f63 725f 7472 616e 736c 6174  ngo-ocr_translat
+000000f0: 6522 0d0a 6479 6e61 6d69 6320 3d20 5b22  e"..dynamic = ["
+00000100: 7665 7273 696f 6e22 5d20 2320 7265 6164  version"] # read
+00000110: 2066 726f 6d20 6f63 725f 7472 616e 736c   from ocr_transl
+00000120: 6174 652f 5f5f 696e 6974 5f5f 2e70 790d  ate/__init__.py.
+00000130: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
+00000140: 446a 616e 676f 2061 7070 2066 6f72 204f  Django app for O
+00000150: 4352 2061 6e64 2074 7261 6e73 6c61 7469  CR and translati
+00000160: 6f6e 220d 0a61 7574 686f 7273 203d 205b  on"..authors = [
+00000170: 0d0a 2020 2020 7b20 6e61 6d65 203d 2022  ..    { name = "
+00000180: 4461 7669 6465 2047 7261 7373 616e 6f22  Davide Grassano"
+00000190: 207d 2c0d 0a5d 0d0a 7265 6164 6d65 203d   },..]..readme =
+000001a0: 2022 5245 4144 4d45 2e6d 6422 0d0a 6c69   "README.md"..li
+000001b0: 6365 6e73 6520 3d20 7b20 6669 6c65 203d  cense = { file =
+000001c0: 2022 4c49 4345 4e53 452e 7478 7422 207d   "LICENSE.txt" }
+000001d0: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+000001e0: 5b0d 0a20 2020 2022 4465 7665 6c6f 706d  [..    "Developm
+000001f0: 656e 7420 5374 6174 7573 203a 3a20 3220  ent Status :: 2 
+00000200: 2d20 5072 652d 416c 7068 6122 2c0d 0a20  - Pre-Alpha",.. 
+00000210: 2020 2022 4672 616d 6577 6f72 6b20 3a3a     "Framework ::
+00000220: 2044 6a61 6e67 6f22 2c0d 0a20 2020 2022   Django",..    "
+00000230: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000240: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
+00000250: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
+00000260: 6365 6e73 6520 7633 2028 4750 4c76 3329  cense v3 (GPLv3)
+00000270: 222c 0d0a 2020 2020 224f 7065 7261 7469  ",..    "Operati
+00000280: 6e67 2053 7973 7465 6d20 3a3a 204d 6963  ng System :: Mic
+00000290: 726f 736f 6674 203a 3a20 5769 6e64 6f77  rosoft :: Window
+000002a0: 7322 2c0d 0a20 2020 2022 4f70 6572 6174  s",..    "Operat
+000002b0: 696e 6720 5379 7374 656d 203a 3a20 504f  ing System :: PO
+000002c0: 5349 5820 3a3a 204c 696e 7578 222c 0d0a  SIX :: Linux",..
+000002d0: 2020 2020 2250 726f 6772 616d 6d69 6e67      "Programming
+000002e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002f0: 686f 6e22 2c0d 0a20 2020 2022 5072 6f67  hon",..    "Prog
+00000300: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000310: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000320: 3130 222c 0d0a 2020 2020 224e 6174 7572  10",..    "Natur
+00000330: 616c 204c 616e 6775 6167 6520 3a3a 2045  al Language :: E
+00000340: 6e67 6c69 7368 222c 0d0a 2020 2020 2254  nglish",..    "T
+00000350: 6f70 6963 203a 3a20 4d75 6c74 696d 6564  opic :: Multimed
+00000360: 6961 203a 3a20 4772 6170 6869 6373 222c  ia :: Graphics",
+00000370: 0d0a 2020 2020 2254 6f70 6963 203a 3a20  ..    "Topic :: 
+00000380: 4461 7461 6261 7365 203a 3a20 4461 7461  Database :: Data
+00000390: 6261 7365 2045 6e67 696e 6573 2f53 6572  base Engines/Ser
+000003a0: 7665 7273 222c 0d0a 2020 2020 2254 6f70  vers",..    "Top
+000003b0: 6963 203a 3a20 5465 7874 2050 726f 6365  ic :: Text Proce
+000003c0: 7373 696e 6720 3a3a 204c 696e 6775 6973  ssing :: Linguis
+000003d0: 7469 6322 2c0d 0a20 2020 2022 496e 7465  tic",..    "Inte
+000003e0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+000003f0: 2045 6e64 2055 7365 7273 2f44 6573 6b74   End Users/Deskt
+00000400: 6f70 222c 0d0a 5d0d 0a6b 6579 776f 7264  op",..]..keyword
+00000410: 7320 3d20 5b22 646a 616e 676f 222c 2022  s = ["django", "
+00000420: 6f63 7222 2c20 2274 7261 6e73 6c61 7469  ocr", "translati
+00000430: 6f6e 225d 0d0a 7265 7175 6972 6573 2d70  on"]..requires-p
+00000440: 7974 686f 6e20 3d20 223e 3d33 2e31 3022  ython = ">=3.10"
+00000450: 0d0a 6465 7065 6e64 656e 6369 6573 203d  ..dependencies =
+00000460: 205b 0d0a 2020 2020 2272 6567 6578 7e3d   [..    "regex~=
+00000470: 3230 3233 2e36 2e33 222c 0d0a 2020 2020  2023.6.3",..    
+00000480: 2272 6571 7565 7374 737e 3d32 2e33 312e  "requests~=2.31.
+00000490: 3022 2c0d 0a20 2020 2022 446a 616e 676f  0",..    "Django
+000004a0: 7e3d 342e 322e 3322 2c0d 0a20 2020 2022  ~=4.2.3",..    "
+000004b0: 5069 6c6c 6f77 7e3d 392e 352e 3022 2c0d  Pillow~=9.5.0",.
+000004c0: 0a20 2020 2022 6f70 656e 6376 2d70 7974  .    "opencv-pyt
+000004d0: 686f 6e2d 6865 6164 6c65 7373 7e3d 342e  hon-headless~=4.
+000004e0: 382e 302e 3734 222c 0d0a 0d0a 2020 2020  8.0.74",....    
+000004f0: 2274 6f72 6368 7e3d 322e 302e 3122 2c0d  "torch~=2.0.1",.
+00000500: 0a20 2020 2022 746f 7263 6876 6973 696f  .    "torchvisio
+00000510: 6e7e 3d30 2e31 352e 3222 2c0d 0a0d 0a20  n~=0.15.2",.... 
+00000520: 2020 2022 7472 616e 7366 6f72 6d65 7273     "transformers
+00000530: 7e3d 342e 3330 2e32 222c 0d0a 2020 2020  ~=4.30.2",..    
+00000540: 2265 6173 796f 6372 7e3d 312e 372e 3022  "easyocr~=1.7.0"
+00000550: 2c0d 0a20 2020 2022 7079 7465 7373 6572  ,..    "pytesser
+00000560: 6163 747e 3d30 2e33 2e31 3022 2c0d 0a20  act~=0.3.10",.. 
+00000570: 2020 2022 6675 6761 7368 697e 3d31 2e32     "fugashi~=1.2
+00000580: 2e31 222c 0d0a 2020 2020 2275 6e69 6469  .1",..    "unidi
+00000590: 632d 6c69 7465 7e3d 312e 302e 3822 2c0d  c-lite~=1.0.8",.
+000005a0: 0a20 2020 2022 7361 6372 656d 6f73 6573  .    "sacremoses
+000005b0: 7e3d 302e 302e 3533 222c 0d0a 2020 2020  ~=0.0.53",..    
+000005c0: 2273 6166 6574 656e 736f 7273 7e3d 302e  "safetensors~=0.
+000005d0: 332e 3122 2c0d 0a20 2020 2022 7365 6e74  3.1",..    "sent
+000005e0: 656e 6365 7069 6563 657e 3d30 2e31 2e39  encepiece~=0.1.9
+000005f0: 3922 2c0d 0a5d 0d0a 0d0a 5b70 726f 6a65  9",..]....[proje
+00000600: 6374 2e75 726c 735d 0d0a 536f 7572 6365  ct.urls]..Source
+00000610: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+00000620: 7562 2e63 6f6d 2f63 7269 7665 6c6c 612f  ub.com/crivella/
+00000630: 6f63 725f 7472 616e 736c 6174 6522 0d0a  ocr_translate"..
+00000640: 0d0a 5b70 726f 6a65 6374 2e6f 7074 696f  ..[project.optio
+00000650: 6e61 6c2d 6465 7065 6e64 656e 6369 6573  nal-dependencies
+00000660: 5d0d 0a6d 7973 716c 203d 205b 0d0a 2020  ]..mysql = [..  
+00000670: 2020 2270 796d 7973 716c 3d3d 312e 312e    "pymysql==1.1.
+00000680: 3022 2c0d 0a5d 0d0a 706f 7374 6772 6573  0",..]..postgres
+00000690: 203d 205b 0d0a 2020 2020 2270 7379 636f   = [..    "psyco
+000006a0: 7067 5b62 696e 6172 795d 3d3d 332e 312e  pg[binary]==3.1.
+000006b0: 3922 2c0d 0a5d 0d0a 7465 7374 7320 3d20  9",..]..tests = 
+000006c0: 5b0d 0a20 2020 2022 7079 7465 7374 222c  [..    "pytest",
+000006d0: 0d0a 2020 2020 2270 7974 6573 742d 636f  ..    "pytest-co
+000006e0: 7622 2c0d 0a20 2020 2022 7079 7465 7374  v",..    "pytest
+000006f0: 2d72 6567 7265 7373 696f 6e73 7e3d 322e  -regressions~=2.
+00000700: 3422 2c0d 0a20 2020 2022 7079 7465 7374  4",..    "pytest
+00000710: 2d64 6a61 6e67 6f7e 3d34 2e35 2e32 222c  -django~=4.5.2",
+00000720: 0d0a 5d0d 0a70 7265 2d63 6f6d 6d69 7420  ..]..pre-commit 
+00000730: 3d20 5b0d 0a20 2020 2022 7072 652d 636f  = [..    "pre-co
+00000740: 6d6d 6974 7e3d 332e 332e 3322 2c0d 0a20  mmit~=3.3.3",.. 
+00000750: 2020 2022 7079 6c69 6e74 7e3d 322e 3137     "pylint~=2.17
+00000760: 2e34 222c 0d0a 2020 2020 2270 796c 696e  .4",..    "pylin
+00000770: 742d 7079 7465 7374 7e3d 312e 312e 3222  t-pytest~=1.1.2"
+00000780: 2c0d 0a20 2020 2022 7079 6c69 6e74 2d64  ,..    "pylint-d
+00000790: 6a61 6e67 6f7e 3d32 2e35 2e33 222c 0d0a  jango~=2.5.3",..
+000007a0: 5d0d 0a72 656c 6561 7365 203d 205b 0d0a  ]..release = [..
+000007b0: 2020 2020 2270 7969 6e73 7461 6c6c 6572      "pyinstaller
+000007c0: 220d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e 666c  "..]....[tool.fl
+000007d0: 6974 2e6d 6f64 756c 655d 0d0a 6e61 6d65  it.module]..name
+000007e0: 203d 2022 6f63 725f 7472 616e 736c 6174   = "ocr_translat
+000007f0: 6522 0d0a 0d0a 5b74 6f6f 6c2e 666c 6974  e"....[tool.flit
+00000800: 2e73 6469 7374 5d0d 0a65 7863 6c75 6465  .sdist]..exclude
+00000810: 203d 205b 0d0a 2020 2020 222e 6769 7469   = [..    ".giti
+00000820: 676e 6f72 6522 2c20 222e 6769 7468 7562  gnore", ".github
+00000830: 222c 0d0a 2020 2020 2269 636f 6e2e 6963  ",..    "icon.ic
+00000840: 6f22 2c20 2272 756e 5f73 6572 7665 722e  o", "run_server.
+00000850: 7079 222c 0d0a 2020 2020 2244 6f63 6b65  py",..    "Docke
+00000860: 7266 696c 6522 2c20 226e 6769 6e78 2e64  rfile", "nginx.d
+00000870: 6566 6175 6c74 222c 2022 7374 6172 742d  efault", "start-
+00000880: 7365 7276 6572 2e73 6822 2c0d 0a20 2020  server.sh",..   
+00000890: 2022 6d79 7369 7465 2f22 2c20 226d 7973   "mysite/", "mys
+000008a0: 6974 652f 2a22 2c20 226d 616e 6167 652e  ite/*", "manage.
+000008b0: 7079 222c 2022 7465 7374 732f 222c 2022  py", "tests/", "
+000008c0: 7465 7374 732f 2a22 2c0d 0a20 2020 205d  tests/*",..    ]
+000008d0: 0d0a 0d0a 5b74 6f6f 6c2e 7079 7465 7374  ....[tool.pytest
+000008e0: 2e69 6e69 5f6f 7074 696f 6e73 5d0d 0a74  .ini_options]..t
+000008f0: 6573 7470 6174 6873 203d 205b 2274 6573  estpaths = ["tes
+00000900: 7473 225d 0d0a 444a 414e 474f 5f53 4554  ts"]..DJANGO_SET
+00000910: 5449 4e47 535f 4d4f 4455 4c45 203d 2022  TINGS_MODULE = "
+00000920: 6d79 7369 7465 2e73 6574 7469 6e67 7322  mysite.settings"
+00000930: 0d0a 6c6f 675f 636c 6920 3d20 310d 0a0d  ..log_cli = 1...
+00000940: 0a5b 746f 6f6c 2e70 796c 696e 742e 6d61  .[tool.pylint.ma
+00000950: 696e 5d0d 0a6c 6f61 642d 706c 7567 696e  in]..load-plugin
+00000960: 7320 3d20 5b0d 0a20 2020 2022 7079 6c69  s = [..    "pyli
+00000970: 6e74 5f64 6a61 6e67 6f22 2c0d 0a20 2020  nt_django",..   
+00000980: 2022 7079 6c69 6e74 5f70 7974 6573 7422   "pylint_pytest"
+00000990: 0d0a 5d0d 0a64 6a61 6e67 6f2d 7365 7474  ..]..django-sett
+000009a0: 696e 6773 2d6d 6f64 756c 6520 3d20 226d  ings-module = "m
+000009b0: 7973 6974 652e 7365 7474 696e 6773 220d  ysite.settings".
+000009c0: 0a0d 0a5b 746f 6f6c 2e70 796c 696e 742e  ...[tool.pylint.
+000009d0: 6d65 7373 6167 6573 5f63 6f6e 7472 6f6c  messages_control
+000009e0: 5d0d 0a64 6973 6162 6c65 203d 205b 0d0a  ]..disable = [..
+000009f0: 2020 2020 226c 6f67 6769 6e67 2d66 7374      "logging-fst
+00000a00: 7269 6e67 2d69 6e74 6572 706f 6c61 7469  ring-interpolati
+00000a10: 6f6e 222c 0d0a 2020 2020 2267 6c6f 6261  on",..    "globa
+00000a20: 6c2d 7374 6174 656d 656e 7422 2c0d 0a20  l-statement",.. 
+00000a30: 2020 2022 6272 6f61 642d 6578 6365 7074     "broad-except
+00000a40: 696f 6e2d 6361 7567 6874 222c 0d0a 2020  ion-caught",..  
+00000a50: 2020 2274 6f6f 2d66 6577 2d70 7562 6c69    "too-few-publi
+00000a60: 632d 6d65 7468 6f64 7322 2c0d 0a5d 0d0a  c-methods",..]..
+00000a70: 0d0a 0d0a 5b74 6f6f 6c2e 7079 6c69 6e74  ....[tool.pylint
+00000a80: 2e66 6f72 6d61 745d 0d0a 6d61 782d 6c69  .format]..max-li
+00000a90: 6e65 2d6c 656e 6774 6820 3d20 3132 300d  ne-length = 120.
+00000aa0: 0a67 6f6f 642d 6e61 6d65 7320 3d20 5b0d  .good-names = [.
+00000ab0: 0a20 2020 2022 5f22 2c0d 0a20 2020 2022  .    "_",..    "
+00000ac0: 6c22 2c20 2272 222c 2022 6222 2c20 2274  l", "r", "b", "t
+00000ad0: 222c 0d0a 2020 2020 226c 3122 2c20 2272  ",..    "l1", "r
+00000ae0: 3122 2c20 2262 3122 2c20 2274 3122 2c0d  1", "b1", "t1",.
+00000af0: 0a20 2020 2022 6c32 222c 2022 7232 222c  .    "l2", "r2",
+00000b00: 2022 6232 222c 2022 7432 222c 0d0a 2020   "b2", "t2",..  
+00000b10: 2020 2269 222c 2022 6a22 2c0d 0a20 2020    "i", "j",..   
+00000b20: 2022 6b22 2c20 2276 222c 0d0a 2020 2020   "k", "v",..    
+00000b30: 2266 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c  "f",..]....[tool
+00000b40: 2e70 796c 696e 742e 6465 7369 676e 5d0d  .pylint.design].
+00000b50: 0a6d 6178 2d61 7267 7320 3d20 3130 0d0a  .max-args = 10..
+00000b60: 6d61 782d 6c6f 6361 6c73 203d 2032 300d  max-locals = 20.
+00000b70: 0a6d 6178 2d61 7474 7269 6275 7465 7320  .max-attributes 
+00000b80: 3d20 3132 0d0a                           = 12..
```

### Comparing `django_ocr_translate-0.1.2/PKG-INFO` & `django_ocr_translate-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ocr_translate
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django app for OCR and translation
 Keywords: django,ocr,translation
 Author: Davide Grassano
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
@@ -14,34 +14,46 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Intended Audience :: End Users/Desktop
-Requires-Dist: regex==2023.6.3
-Requires-Dist: requests==2.31.0
-Requires-Dist: Django==4.2.2
-Requires-Dist: Pillow==9.5.0
-Requires-Dist: opencv-python-headless==4.8.0.74
-Requires-Dist: torch==2.0.1
-Requires-Dist: torchvision==0.15.2
-Requires-Dist: transformers==4.30.2
-Requires-Dist: easyocr==1.7.0
-Requires-Dist: pytesseract==0.3.10
-Requires-Dist: fugashi==1.2.1
-Requires-Dist: unidic-lite==1.0.8
-Requires-Dist: sacremoses==0.0.53
-Requires-Dist: safetensors==0.3.1
-Requires-Dist: sentencepiece==0.1.99
+Requires-Dist: regex~=2023.6.3
+Requires-Dist: requests~=2.31.0
+Requires-Dist: Django~=4.2.3
+Requires-Dist: Pillow~=9.5.0
+Requires-Dist: opencv-python-headless~=4.8.0.74
+Requires-Dist: torch~=2.0.1
+Requires-Dist: torchvision~=0.15.2
+Requires-Dist: transformers~=4.30.2
+Requires-Dist: easyocr~=1.7.0
+Requires-Dist: pytesseract~=0.3.10
+Requires-Dist: fugashi~=1.2.1
+Requires-Dist: unidic-lite~=1.0.8
+Requires-Dist: sacremoses~=0.0.53
+Requires-Dist: safetensors~=0.3.1
+Requires-Dist: sentencepiece~=0.1.99
 Requires-Dist: pymysql==1.1.0 ; extra == "mysql"
 Requires-Dist: psycopg[binary]==3.1.9 ; extra == "postgres"
+Requires-Dist: pre-commit~=3.3.3 ; extra == "pre-commit"
+Requires-Dist: pylint~=2.17.4 ; extra == "pre-commit"
+Requires-Dist: pylint-pytest~=1.1.2 ; extra == "pre-commit"
+Requires-Dist: pylint-django~=2.5.3 ; extra == "pre-commit"
+Requires-Dist: pyinstaller ; extra == "release"
+Requires-Dist: pytest ; extra == "tests"
+Requires-Dist: pytest-cov ; extra == "tests"
+Requires-Dist: pytest-regressions~=2.4 ; extra == "tests"
+Requires-Dist: pytest-django~=4.5.2 ; extra == "tests"
 Project-URL: Source, https://github.com/crivella/ocr_translate
 Provides-Extra: mysql
 Provides-Extra: postgres
+Provides-Extra: pre-commit
+Provides-Extra: release
+Provides-Extra: tests
 
 # OCR_translate
 
 This is a Django app for creating back-end server aimed at performing OCR and translation of images received via a POST request.
 
 The OCR and translation is performed using freely available machine learning models and packages (see below for what is currently implemented).
 
@@ -88,14 +100,32 @@
 
 - manually edit the [settings.py](mysite/settings.py)
 - Use the provided [Environment variables](#environment-variables)
 See below for a [list of supported databases](#supported-databases)
 
 You will also have to modify the `ALLOWED_HOSTS` in case you plan to access the server from somewhere other than *localhost*.
 
+### From Release file
+
+(Tested on Windows 11)
+From the github releases you can download either:
+
+- The [CPU only version](/releases/latest/download/run_server-cpu.exe)
+- The GPU version split in [file 1](/releases/latest/download/run_server-gpu.zip.001) and [file 2](/releases/latest/download/run_server-gpu.zip.002) (The CUDA dependencies makes it take much more space), wich can be restored using tools like [7zip](https://www.7-zip.org/https://www.7-zip.org/) and [NanaZip](https://github.com/M2Team/NanaZip).
+
+Not that every time you run the EXE, it will decompress itself into a temporary folder so:
+
+- The exe will appear as an empty console until all the file are extracted and the actual script start running.
+- By launching the server multiple times without restarting (especially the GPU one), you risk quickly filling up your drive
+
+You can either just start the server and it will run with sensible defaults. Most notably the models files and database will be downloaded/created under `%userprofile%/.ocr_translate`.
+Also the gpu version will attempt to run on GPU by default, and fall-back to CPU if the former is not available.
+
+For customization, you can set the [environment variable](#environment-variables) yourself, either via powershell or by searching for *environment variable* in the settings menu
+
 ### From Github installation
 
 The Github repo provides not only the Django app files, but also the already configured project files used to start the server.
 
 Create/Initialize your database by running
 
 - `python manage.py migrate`
@@ -212,7 +242,8 @@
 | `DATABASE_PASSWORD` | optional | Probably required if using another db back-end |
 
 ## Supported databases
 
 - [SQLite](https://www.sqlite.org/index.html) This is mostly fine for a self-hosted server accessed by a single  or few users (and it's probably gonna be faster than any other database not running on the same network as the server because of latency).
 - [Postgresql](https://www.postgresql.org/)
 - [MySQL](https://www.mysql.com)/[MariaDB](https://mariadb.org/)
+
```

