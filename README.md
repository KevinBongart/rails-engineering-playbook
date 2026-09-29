# Rails Engineering Playbook

The shared engineering standards for the Ruby on Rails applications that adopt
this repository. [`PLAYBOOK.md`](PLAYBOOK.md) is the whole document.

It covers architecture, Ruby and Rails conventions, database design, frontend
and interaction design, testing strategy, security and privacy, dependencies,
continuous integration, deployment and operations, documentation architecture,
the product development workflow, agentic editing standards, and a definition of
done.

## Using it from an application

Clone this repository as a sibling of the application repositories that
reference it:

```sh
cd ~/your/code/directory
git clone git@github.com:KevinBongart/rails-engineering-playbook.git
```

Each adopting application's `AGENTS.md` or `CLAUDE.md` points here and describes
only its own truth: stack, domain model, commands, boundaries, and roadmap. The
playbook describes the preferred direction. It does not assert that its preferred
stack or checks are already installed in any given application — treat a gap as
work to be scheduled, not as a description of what is there.

Pull the latest copy before relying on it:

```sh
git -C ../rails-engineering-playbook pull --ff-only
```

## Contributing

`PLAYBOOK.md` has a "Maintaining this playbook" section that governs changes.
In short: put cross-application insights here and application-specific truth in
that application's own reference, motivate each guideline with the concrete
experience behind it, and keep every example in an invented domain.

**Never** paste a real schema, table name, hostname, credential, customer
identifier, or private business rule into this repository, including inside an
illustrative code block.
