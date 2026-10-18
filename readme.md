# Getting Started

Welcome to your new CAP project.

It contains these folders and files, following our recommended project layout:

| File or Folder | Purpose                              |
| -------------- | ------------------------------------ |
| `app/`         | content for UI frontends goes here   |
| `db/`          | your domain models and data go here  |
| `srv/`         | your service models and code go here |
| `readme.md`    | this getting started guide           |

## Next Steps

- Open a new terminal and run `cds watch`
- (in VS Code simply choose _**Terminal** > Run Task > cds watch_)
- Start with your domain model, in a CDS file in `db/`

## Learn More

Learn more at <https://cap.cloud.sap>.

commit and push to feature/CAP-1234-new-feature:
----------------------------------------------------------------------------------------------

git add .
git commit -m "chore(package): release workflow" -m "release workflow" -m "Refs: CAP-1262"
git push origin feature/CAP-1234-new-feature

build:
----------------------------------------------------------------------------------------------

npx mbt build --mtar blackmores-o2i-sales-order-management

deploy:
----------------------------------------------------------------------------------------------

cf deploy mta_archives/blackmores-o2i-sales-order-management.mtar \
-e config/mtaext/dev.mtaext
