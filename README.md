# NAME

Database::Migrator::Pg - Database::Migrator implementation for Postgres

# VERSION

version 0.06

# SYNOPSIS

    package MyApp::Migrator;

    use Moose;

    extends 'Database::Migrator::Pg';

    has '+database' => (
        required => 0,
        default  => 'MyApp',
    );

# DESCRIPTION

This module provides a [Database::Migrator](https://metacpan.org/pod/Database::Migrator) implementation for Postgres. See
[Database::Migrator](https://metacpan.org/pod/Database::Migrator) and [Database::Migrator::Core](https://metacpan.org/pod/Database::Migrator::Core) for more documentation.

# ATTRIBUTES

This class adds several attributes in addition to those implemented by
[Database::Migrator::Core](https://metacpan.org/pod/Database::Migrator::Core). All of these attributes are optional.

- encoding

    The encoding of the database. This is only used when creating a new
    database.

- locale

    The locale of the database. This is only used when creating a new
    database.

- lc\_collate

    The LC\_COLLATE setting for the database. This is only used when creating a new
    database.

- lc\_ctype

    The LC\_CTYPE setting for the database. This is only used when creating a new
    database.

- owner

    The owner of the database. This is only used when creating a new
    database.

- tablespace

    The tablespace for the database. This is only used when creating a new
    database.

- template

    The template for the database. This is only used when creating a new database.

# SUPPORT

Please submit bugs to the CPAN RT system at
http://rt.cpan.org/NoAuth/Bugs.html?Dist=Database-Migrator-Pg or via email at
bug-database-migrator-pg@rt.cpan.org.

Bugs may be submitted through [the RT bug tracker](http://rt.cpan.org/Public/Dist/Display.html?Name=Database-Migrator-Pg)
(or [bug-database-migrator-pg@rt.cpan.org](mailto:bug-database-migrator-pg@rt.cpan.org)).

I am also usually active on IRC as 'drolsky' on `irc://irc.perl.org`.

# AUTHOR

Dave Rolsky &lt;autarch@urth.org>

# COPYRIGHT AND LICENCE

This software is Copyright (c) 2016 by MaxMind, Inc.

This is free software, licensed under:

    The Artistic License 2.0 (GPL Compatible)
