```dataview
table category, status, asigned_to
from "sheets"
where !contains(file.path, "sheets/Control")
